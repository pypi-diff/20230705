# Comparing `tmp/django-pfx-1.2.dev90.tar.gz` & `tmp/django-pfx-1.2.dev92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pfx-1.2.dev90.tar", last modified: Tue Jul  4 11:52:10 2023, max compression
+gzip compressed data, was "django-pfx-1.2.dev92.tar", last modified: Wed Jul  5 14:41:45 2023, max compression
```

## Comparing `django-pfx-1.2.dev90.tar` & `django-pfx-1.2.dev92.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.205080 django-pfx-1.2.dev90/django_pfx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1692 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 11:52:10.000000 django-pfx-1.2.dev90/django_pfx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.206081 django-pfx-1.2.dev90/img/
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/img/pfx.png
--rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/img/pfx.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.206081 django-pfx-1.2.dev90/pfx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.208080 django-pfx-1.2.dev90/pfx/pfxcore/
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.208080 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apidoc/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.209081 django-pfx-1.2.dev90/pfx/pfxcore/decorator/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/decorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2530 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/decorator/rest.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.209081 django-pfx-1.2.dev90/pfx/pfxcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/http/json_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.200080 django-pfx-1.2.dev90/pfx/pfxcore/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.200080 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)     3331 2023-07-04 11:52:05.000000 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.210080 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/management/commands/makeapidoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.211080 django-pfx-1.2.dev90/pfx/pfxcore/middleware/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/middleware/locale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.212081 django-pfx-1.2.dev90/pfx/pfxcore/models/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/cache_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/not_null_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/pfx_models.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/models/user_filtered_queryset_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.212081 django-pfx-1.2.dev90/pfx/pfxcore/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/serializers/json.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.213081 django-pfx-1.2.dev90/pfx/pfxcore/storage/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/storage/s3_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.201080 django-pfx-1.2.dev90/pfx/pfxcore/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.214080 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/welcome_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/templates/registration/welcome_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/test.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.215080 django-pfx-1.2.dev90/pfx/pfxcore/views/
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15850 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/authentication_views.py
--rw-rw-rw-   0 root         (0) root         (0)    12339 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/filters_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/locale_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.219081 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/date_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_count.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_items.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_order.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_search.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/media_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_filters.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/meta_orders.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_limit.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_offset.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page_size.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset_page_subset.py
--rw-rw-rw-   0 root         (0) root         (0)    28550 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pfx/pfxcore/views/rest_views.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/runtest.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.220080 django-pfx-1.2.dev90/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.221080 django-pfx-1.2.dev90/tests/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/common.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev_custom_example.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/settings/dev_default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 11:52:10.225080 django-pfx-1.2.dev90/tests/tests/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/basic_api_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/basic_api_test.py
--rw-rw-rw-   0 root         (0) root         (0)    19712 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_api_doc.py
--rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_auth_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_locale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_perm_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_perms_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_shortcuts.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_timezone_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_user_queryset.py
--rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_view_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/tests/test_view_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8416 2023-07-04 11:51:25.000000 django-pfx-1.2.dev90/tests/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.890003 django-pfx-1.2.dev92/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-05 14:41:45.890003 django-pfx-1.2.dev92/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.871003 django-pfx-1.2.dev92/django_pfx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-07-05 14:41:45.000000 django-pfx-1.2.dev92/django_pfx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-07-05 14:41:45.000000 django-pfx-1.2.dev92/django_pfx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:41:45.000000 django-pfx-1.2.dev92/django_pfx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-05 14:41:45.000000 django-pfx-1.2.dev92/django_pfx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 14:41:45.000000 django-pfx-1.2.dev92/django_pfx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.871003 django-pfx-1.2.dev92/img/
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/img/pfx.png
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/img/pfx.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.871003 django-pfx-1.2.dev92/pfx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.874003 django-pfx-1.2.dev92/pfx/pfxcore/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.874003 django-pfx-1.2.dev92/pfx/pfxcore/apidoc/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/apidoc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/apidoc/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/apidoc/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/apidoc/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.875003 django-pfx-1.2.dev92/pfx/pfxcore/decorator/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/decorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/decorator/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.875003 django-pfx-1.2.dev92/pfx/pfxcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/http/json_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.865003 django-pfx-1.2.dev92/pfx/pfxcore/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.865003 django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.876003 django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-07-05 14:41:41.000000 django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     5332 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.876003 django-pfx-1.2.dev92/pfx/pfxcore/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.876003 django-pfx-1.2.dev92/pfx/pfxcore/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/management/commands/makeapidoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.877003 django-pfx-1.2.dev92/pfx/pfxcore/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/middleware/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/middleware/locale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.878003 django-pfx-1.2.dev92/pfx/pfxcore/models/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/models/cache_mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/models/not_null_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3419 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/models/pfx_models.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/models/user_filtered_queryset_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.878003 django-pfx-1.2.dev92/pfx/pfxcore/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/serializers/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.879003 django-pfx-1.2.dev92/pfx/pfxcore/storage/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/storage/s3_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.866003 django-pfx-1.2.dev92/pfx/pfxcore/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.880003 django-pfx-1.2.dev92/pfx/pfxcore/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/templates/registration/welcome_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/templates/registration/welcome_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)    10198 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.881003 django-pfx-1.2.dev92/pfx/pfxcore/views/
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15850 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/authentication_views.py
+-rw-rw-rw-   0 root         (0) root         (0)    13642 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/filters_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/locale_views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.885003 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/date_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_count.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_items.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_order.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_search.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/media_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/meta_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/meta_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/meta_orders.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset_offset.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset_page_size.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset_page_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)    28550 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pfx/pfxcore/views/rest_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      440 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/runtest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-05 14:41:45.891003 django-pfx-1.2.dev92/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.885003 django-pfx-1.2.dev92/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6698 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.886003 django-pfx-1.2.dev92/tests/settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/dev_custom_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/settings/dev_default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:41:45.890003 django-pfx-1.2.dev92/tests/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/basic_api_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    46979 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/basic_api_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    20542 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_api_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)    29106 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_auth_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     4221 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     9909 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_locale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_perm_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3725 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_perms_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_shortcuts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_timezone_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_user_queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3558 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_view_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7356 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/tests/test_view_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8656 2023-07-05 14:41:04.000000 django-pfx-1.2.dev92/tests/views.py
```

### Comparing `django-pfx-1.2.dev90/.gitlab-ci.yml` & `django-pfx-1.2.dev92/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/LICENSE` & `django-pfx-1.2.dev92/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/PKG-INFO` & `django-pfx-1.2.dev92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev90
+Version: 1.2.dev92
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev90/README.md` & `django-pfx-1.2.dev92/README.md`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/django_pfx.egg-info/PKG-INFO` & `django-pfx-1.2.dev92/django_pfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pfx
-Version: 1.2.dev90
+Version: 1.2.dev92
 Summary: Django PFX is a toolkit to build web APIs dedicated to be used by React progressive web app.
 Author: Hervé Martinet
 Author-email: herve.martinet@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://gitlab.com/hmartinet/django-pfx
 Project-URL: Tracker, https://gitlab.com/hmartinet/django-pfx/-/issues
 Classifier: Environment :: Web Environment
```

### Comparing `django-pfx-1.2.dev90/django_pfx.egg-info/SOURCES.txt` & `django-pfx-1.2.dev92/django_pfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/img/pfx.png` & `django-pfx-1.2.dev92/img/pfx.png`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/img/pfx.svg` & `django-pfx-1.2.dev92/img/pfx.svg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/apidoc/parameters.py` & `django-pfx-1.2.dev92/pfx/pfxcore/apidoc/parameters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/apidoc/schema.py` & `django-pfx-1.2.dev92/pfx/pfxcore/apidoc/schema.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/decorator/rest.py` & `django-pfx-1.2.dev92/pfx/pfxcore/decorator/rest.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/exceptions.py` & `django-pfx-1.2.dev92/pfx/pfxcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/fields.py` & `django-pfx-1.2.dev92/pfx/pfxcore/fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo` & `django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po` & `django-pfx-1.2.dev92/pfx/pfxcore/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/management/commands/makeapidoc.py` & `django-pfx-1.2.dev92/pfx/pfxcore/management/commands/makeapidoc.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/middleware/authentication.py` & `django-pfx-1.2.dev92/pfx/pfxcore/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/middleware/locale.py` & `django-pfx-1.2.dev92/pfx/pfxcore/middleware/locale.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/models/cache_mixins.py` & `django-pfx-1.2.dev92/pfx/pfxcore/models/cache_mixins.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/models/pfx_models.py` & `django-pfx-1.2.dev92/pfx/pfxcore/models/pfx_models.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/shortcuts.py` & `django-pfx-1.2.dev92/pfx/pfxcore/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/storage/s3_storage.py` & `django-pfx-1.2.dev92/pfx/pfxcore/storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/test.py` & `django-pfx-1.2.dev92/pfx/pfxcore/test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/__init__.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/authentication_views.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/authentication_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/fields.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from django.db import models
 from django.db.models.constants import LOOKUP_SEP
 from django.utils.formats import date_format
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 
+from apispec.utils import deepupdate
 from apispec.yaml_utils import load_yaml_from_docstring
 
 from pfx.pfxcore import fields as pfx_fields
 from pfx.pfxcore.shortcuts import get_object
 
 logger = logging.getLogger(__name__)
 
@@ -218,21 +219,22 @@
         elif self.field_type == FieldType.ModelObject:
             properties = {}
             if self.related_model:
                 res['format'] = str(self.related_model._meta.verbose_name)
                 properties.update(self.related_model.json_repr_schema())
                 doc = inspect.getdoc(self.related_model.json_repr)
                 if doc:
-                    properties.update(load_yaml_from_docstring(doc))
+                    properties = deepupdate(
+                        load_yaml_from_docstring(doc), properties)
             if self.json_repr:
                 doc = inspect.getdoc(self.json_repr)
                 if doc:
                     p = load_yaml_from_docstring(doc)
                     if p.pop('_extends', False):
-                        properties.update(p)
+                        properties = deepupdate(p, properties)
                     else:
                         properties = p
             if properties:
                 if request:
                     res.pop('type', None)
                     res.pop('format', None)
                     res['oneOf'] = [
@@ -241,14 +243,41 @@
                              properties=dict(pk=properties.get('pk')))]
                 else:
                     res['properties'] = properties
         elif self.field_type == FieldType.MinutesDurationField:
             res = pfx_fields.MinutesDurationField.schema
         elif self.field_type == FieldType.ModelObjectList:
             res['items'] = dict(type='object')
+            properties = {}
+            if self.related_model:
+                res['items']['format'] = str(
+                    self.related_model._meta.verbose_name)
+                properties.update(self.related_model.json_repr_schema())
+                doc = inspect.getdoc(self.related_model.json_repr)
+                if doc:
+                    properties = deepupdate(
+                        load_yaml_from_docstring(doc), properties)
+            if self.json_repr:
+                doc = inspect.getdoc(self.json_repr)
+                if doc:
+                    p = load_yaml_from_docstring(doc)
+                    if p.pop('_extends', False):
+                        properties = deepupdate(p, properties)
+                    else:
+                        properties = p
+            if properties:
+                if request:
+                    res.pop('type', None)
+                    res.pop('format', None)
+                    res['oneOf'] = [
+                        properties.get('pk'),
+                        dict(type='object',
+                             properties=dict(pk=properties.get('pk')))]
+                else:
+                    res['items']['properties'] = properties
         res['readonly'] = self.readonly_create and self.readonly_update
         if self.choices:
             res['enum'] = list(self.choices)
         return res
 
 
 class ViewModelField(ViewField):
```

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/filters_views.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/filters_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/locale_views.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/locale_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/__init__.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/date_format.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/date_format.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/groups.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/groups.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/list_order.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/list_order.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/parameters/subset.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/parameters/subset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/pfx/pfxcore/views/rest_views.py` & `django-pfx-1.2.dev92/pfx/pfxcore/views/rest_views.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/setup.cfg` & `django-pfx-1.2.dev92/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/models.py` & `django-pfx-1.2.dev92/tests/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -197,7 +197,15 @@
             UniqueConstraint(
                 fields=['author', 'name'],
                 name='book_unique_author_and_name',
                 message="%(name)s already exists for %(author)s")]
 
     def __str__(self):
         return f"{self.name}"
+
+    def json_repr(self, **values):
+        """JSON representation.
+        ---
+        author_name:
+            type: string
+        """
+        return super().json_repr(author_name=str(self.author), **values)
```

### Comparing `django-pfx-1.2.dev90/tests/settings/common.py` & `django-pfx-1.2.dev92/tests/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/settings/dev_custom_example.py` & `django-pfx-1.2.dev92/tests/settings/dev_custom_example.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/__init__.py` & `django-pfx-1.2.dev92/tests/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/basic_api_errors.py` & `django-pfx-1.2.dev92/tests/tests/basic_api_errors.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/basic_api_test.py` & `django-pfx-1.2.dev92/tests/tests/basic_api_test.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_api_doc.py` & `django-pfx-1.2.dev92/tests/tests/test_api_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,31 @@
         self.assertJE(props, 'last_name.type', 'string')
         self.assertJE(props, 'last_name.readonly', False)
         self.assertJE(props, 'gender.type', 'string')
         self.assertJE(props, 'gender.enum', ['male', 'female'])
 
         schema_key = self.get_val(
             paths,
+            '/authors-annotate/{pk}.get.responses.200.content'
+            '.application/json.schema'
+        )['$ref'].split('/')[-1]
+        # Check ModelObjectList fields
+        props = spec['components']['schemas'][schema_key]['properties']
+        self.assertJE(props, 'books.type', 'array')
+        self.assertJE(props, 'books.items.type', 'object')
+        self.assertJE(props, 'books.items.format', 'Book')
+        props = self.get_val(props, 'books.items.properties')
+        self.assertJE(props, 'pk.type', 'number')
+        self.assertJE(props, 'resource_name.type', 'string')
+        self.assertJE(props, 'resource_reference.type', 'string')
+        self.assertJE(props, 'author_name.type', 'string')
+        self.assertJE(props, 'author_gender.type', 'string')
+
+        schema_key = self.get_val(
+            paths,
             '/books-custom-author/{pk}.get.responses.200.content'
             '.application/json.schema'
         )['$ref'].split('/')[-1]
         self.assertIn("Book", schema_key)
         props = spec['components']['schemas'][schema_key]['properties']
         # Check VF field with alias
         self.assertJE(props, 'book_name.type', 'string')
```

### Comparing `django-pfx-1.2.dev90/tests/tests/test_auth_api.py` & `django-pfx-1.2.dev92/tests/tests/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_cache.py` & `django-pfx-1.2.dev92/tests/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_fields.py` & `django-pfx-1.2.dev92/tests/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_filters.py` & `django-pfx-1.2.dev92/tests/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_locale_api.py` & `django-pfx-1.2.dev92/tests/tests/test_locale_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_perm_tests.py` & `django-pfx-1.2.dev92/tests/tests/test_perm_tests.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_perms_api.py` & `django-pfx-1.2.dev92/tests/tests/test_perms_api.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_shortcuts.py` & `django-pfx-1.2.dev92/tests/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_timezone_middleware.py` & `django-pfx-1.2.dev92/tests/tests/test_timezone_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_tools.py` & `django-pfx-1.2.dev92/tests/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_user_queryset.py` & `django-pfx-1.2.dev92/tests/tests/test_user_queryset.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_view_decorators.py` & `django-pfx-1.2.dev92/tests/tests/test_view_decorators.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/tests/test_view_fields.py` & `django-pfx-1.2.dev92/tests/tests/test_view_fields.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/urls.py` & `django-pfx-1.2.dev92/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-pfx-1.2.dev90/tests/views.py` & `django-pfx-1.2.dev92/tests/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,19 +121,30 @@
         return JsonResponse(dict(value='static:less'))
 
     @rest_api("/priority/priority-more", method="get", priority=1)
     def priority_test3(self, *args, **kwargs):
         return JsonResponse(dict(value='static:more'))
 
 
+def books_json_repr(book):
+    """JSON representation.
+    ---
+    _extends: true
+    author_gender:
+        type: string
+    """
+    return book.json_repr(author_gender=book.author.gender)
+
+
 @rest_doc('/<int:id>', 'get', summary="Get custom author", groups=["custom"])
 @rest_view("/authors-annotate")
 class AuthorAnnotateRestView(AuthorRestView):
     fields = [
         'first_name', 'last_name', 'slug',
+        VF('books', json_repr=books_json_repr),
         'books_count', 'books_count_annotate', 'books_count_prop']
     list_fields = [
         'first_name', 'last_name', 'slug',
         'books_count', 'books_count_annotate', 'books_count_prop']
 
     def get_queryset(self):
         return super().get_queryset().annotate(
```

