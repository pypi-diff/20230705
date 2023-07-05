# Comparing `tmp/django-listing-0.0.9.tar.gz` & `tmp/django-listing-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-listing-0.0.9.tar", last modified: Tue Nov  9 08:54:01 2021, max compression
+gzip compressed data, was "django-listing-0.5.0.tar", last modified: Wed Jul  5 12:43:18 2023, max compression
```

## Comparing `django-listing-0.0.9.tar` & `django-listing-0.5.0.tar`

### file list

```diff
@@ -1,93 +1,234 @@
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/dependency_links.txt
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)        1 2020-07-24 15:40:15.000000 django-listing-0.0.9/django_listing.egg-info/not-zip-safe
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)       55 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/requires.txt
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)     5410 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/PKG-INFO
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)       15 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/top_level.txt
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)     3341 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      234 2021-11-09 08:50:06.000000 django-listing-0.0.9/CHANGES.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2021-11-09 08:54:00.000000 django-listing-0.0.9/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      982 2021-04-01 07:22:20.000000 django-listing-0.0.9/LICENSE.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1928 2020-07-24 13:34:19.000000 django-listing-0.0.9/setup.py
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/fr/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5410 2020-05-15 07:06:48.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      379 2020-05-15 07:06:39.000000 django-listing-0.0.9/django_listing/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/en/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5411 2020-05-15 07:06:44.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      380 2020-05-15 07:06:39.000000 django-listing-0.0.9/django_listing/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    17683 2020-07-24 13:34:19.000000 django-listing-0.0.9/django_listing/filters.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10991 2020-05-20 12:15:51.000000 django-listing-0.0.9/django_listing/record.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      622 2021-11-09 08:50:06.000000 django-listing-0.0.9/django_listing/__init__.py
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templatetags/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templatetags/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11013 2021-02-22 12:43:13.000000 django-listing-0.0.9/django_listing/templatetags/django_listing.py
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templates/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/templates/django_listing/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13292 2021-08-19 06:39:39.000000 django-listing-0.0.9/django_listing/templates/django_listing/paginator.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2020-05-19 13:04:26.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_dropdown.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_update.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2759 2020-05-17 09:45:41.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_variations.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2018-05-13 07:49:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/div_row.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1785 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/action_footer.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6309 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/templates/django_listing/toolbar.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1843 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/footer.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      452 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/header.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      226 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/empty_listing.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/templates/django_listing/selection_overlay.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1405 2020-05-29 10:15:29.000000 django-listing-0.0.9/django_listing/templates/django_listing/view_object_popup.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1982 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/templates/django_listing/filters_form.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1188 2018-06-21 08:12:52.000000 django-listing-0.0.9/django_listing/templates/django_listing/listing_div.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-05-19 13:04:19.000000 django-listing-0.0.9/django_listing/templates/django_listing/tbi_select.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      824 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/templates/django_listing/action_header.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1750 2021-08-23 13:08:34.000000 django-listing-0.0.9/django_listing/templates/django_listing/actions_buttons.html
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1226 2018-04-26 06:48:47.000000 django-listing-0.0.9/django_listing/context.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2031 2021-08-20 07:33:53.000000 django-listing-0.0.9/django_listing/utils.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    42360 2021-08-23 15:51:02.000000 django-listing-0.0.9/django_listing/listing.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7396 2018-04-26 06:48:47.000000 django-listing-0.0.9/django_listing/aggregations.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    17977 2021-08-23 15:51:02.000000 django-listing-0.0.9/django_listing/views.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7851 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/listing_form.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    41819 2021-08-20 15:32:45.000000 django-listing-0.0.9/django_listing/columns.py
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/js/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10551 2021-08-19 14:55:45.000000 django-listing-0.0.9/django_listing/static/django_listing/js/django_listing.js
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/csv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/json.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/xlsx.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/pdf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/dbf.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/xls.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/tsv.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/html.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/icons/ods.svg
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/css/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-embedded.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7-codes.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32713 2021-08-20 07:03:29.000000 django-listing-0.0.9/django_listing/static/django_listing/css/django_listing.css
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.0.9/django_listing/static/django_listing/css/animation.css
-drwxr-xr-x   0 elapouya  (1000) elapouya  (1000)        0 2021-11-09 08:54:00.000000 django-listing-0.0.9/django_listing/static/django_listing/font/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.eot
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.svg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.ttf
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff2
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1841 2021-02-22 10:27:58.000000 django-listing-0.0.9/django_listing/app_settings.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      631 2018-07-26 15:34:44.000000 django-listing-0.0.9/django_listing/exceptions.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2019-08-27 07:31:28.000000 django-listing-0.0.9/django_listing/apps.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10088 2020-08-13 07:02:47.000000 django-listing-0.0.9/django_listing/toolbar.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1725 2018-05-27 16:03:20.000000 django-listing-0.0.9/django_listing/html_attributes.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12882 2021-08-23 14:09:39.000000 django-listing-0.0.9/django_listing/actions_buttons_column.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8239 2021-08-19 06:44:22.000000 django-listing-0.0.9/django_listing/paginators.py
--rw-r--r--   0 elapouya  (1000) elapouya  (1000)     5410 2021-11-09 08:54:00.000000 django-listing-0.0.9/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3639 2020-07-24 13:34:19.000000 django-listing-0.0.9/README.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-05-30 19:21:14.000000 django-listing-0.0.9/MANIFEST.in
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.727556 django-listing-0.5.0/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1578 2023-07-05 12:41:48.000000 django-listing-0.5.0/CHANGES.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      982 2021-04-01 07:22:20.000000 django-listing-0.5.0/LICENSE.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      215 2020-05-30 19:21:14.000000 django-listing-0.5.0/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6359 2023-07-05 12:43:18.727556 django-listing-0.5.0/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3742 2023-05-08 12:05:07.000000 django-listing-0.5.0/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      698 2023-07-05 12:41:48.000000 django-listing-0.5.0/django_listing/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15629 2023-07-05 10:36:54.000000 django-listing-0.5.0/django_listing/actions_buttons_column.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7260 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/aggregations.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3373 2023-06-27 11:53:27.000000 django-listing-0.5.0/django_listing/apps.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    50691 2023-06-20 14:05:27.000000 django-listing-0.5.0/django_listing/columns.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1230 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/context.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      695 2023-02-03 14:07:52.000000 django-listing-0.5.0/django_listing/exceptions.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    27967 2023-06-28 07:03:56.000000 django-listing-0.5.0/django_listing/filters.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1706 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/html_attributes.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    46156 2023-06-28 05:36:02.000000 django-listing-0.5.0/django_listing/listing.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7944 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/listing_form.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.707556 django-listing-0.5.0/django_listing/locale/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.707556 django-listing-0.5.0/django_listing/locale/en/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      527 2023-04-21 13:36:28.000000 django-listing-0.5.0/django_listing/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8395 2023-04-21 13:36:00.000000 django-listing-0.5.0/django_listing/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.707556 django-listing-0.5.0/django_listing/locale/fr/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6571 2023-06-23 15:25:23.000000 django-listing-0.5.0/django_listing/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10804 2023-06-23 15:23:24.000000 django-listing-0.5.0/django_listing/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9140 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/paginators.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11731 2023-06-28 07:51:37.000000 django-listing-0.5.0/django_listing/record.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.707556 django-listing-0.5.0/django_listing/static/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.711556 django-listing-0.5.0/django_listing/static/django_listing/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.707556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/animation.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32396 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.eot
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.woff
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/csv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/dbf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/html.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/json.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/ods.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/pdf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/tsv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/xls.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.711556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    19701 2023-04-30 16:37:00.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/_fonts.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13162 2023-06-26 10:45:48.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/_main.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1857 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/animation.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4790 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_accordion.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2126 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_alert.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1118 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_badge.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      911 2023-05-03 12:10:03.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_bootstrap.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1751 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_breadcrumb.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3073 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_button-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6685 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_buttons.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6736 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_card.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5580 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_carousel.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1127 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_close.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1201 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_containers.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8018 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_dropdown.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      256 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_forms.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10554 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_functions.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      575 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      294 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_helpers.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1158 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_images.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6475 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_list-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1648 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_maps.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      899 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_mixins.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7762 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_modal.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4665 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_nav.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8936 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_navbar.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4555 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_offcanvas.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3940 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_pagination.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      859 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_placeholders.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6907 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_popover.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1875 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_progress.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12311 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_reboot.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2395 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_root.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2429 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_spinners.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4358 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tables.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2490 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_toasts.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3939 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_tooltip.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      425 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_transitions.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1420 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_type.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    14817 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_utilities.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    68610 2023-05-03 10:46:06.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/_variables.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1198 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      163 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-reboot.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      280 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/bootstrap-utilities.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2030 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_floating-labels.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4287 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-check.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5695 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-control.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2796 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-range.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2316 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-select.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      219 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_form-text.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3835 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_input-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1142 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_labels.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      478 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/forms/_validation.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       37 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_clearfix.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      454 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_color-bg.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      450 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_colored-links.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      621 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_position.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      399 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_ratio.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      245 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stacks.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      223 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_stretched-link.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       73 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_text-truncation.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      136 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_visually-hidden.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/helpers/_vr.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      393 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_alert.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      328 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_backdrop.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      263 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_banner.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2031 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_border-radius.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      398 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_box-shadow.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4580 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_breakpoints.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3220 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_buttons.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1473 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_caret.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      147 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_clearfix.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      167 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_color-scheme.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      410 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_container.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      613 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_deprecate.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4122 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_forms.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1956 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_gradients.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4726 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_grid.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      395 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_image.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      509 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_list-group.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_lists.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      387 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_pagination.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      495 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_reset-text.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_resize.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1101 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_table-variants.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      168 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_text-truncate.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      661 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_transition.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3380 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_utilities.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1012 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/mixins/_visually-hidden.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1737 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/utilities/_api.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.719556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10029 2022-11-21 18:19:01.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/bootstrap/vendor/_rfs.scss
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     8452 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74922 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing-embedded.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15031 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7-codes.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    15304 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing-ie7.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    33720 2023-06-26 10:45:49.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     7269 2023-06-26 10:45:49.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing.css.map
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    25343 2023-06-26 10:45:50.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      439 2023-05-05 07:38:04.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/css/django_listing.scss
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74488 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/django_listing.eot
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    99231 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/django_listing.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    74296 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/django_listing.ttf
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    40228 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/django_listing.woff
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    32996 2020-05-06 06:54:52.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/font/django_listing.woff2
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1137 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/csv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1721 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/dbf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1171 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/html.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2109 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/json.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3686 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/ods.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1502 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/pdf.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      989 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/tsv.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      948 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/xls.svg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1086 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/static/django_listing/bootstrap5/icons/xlsx.svg
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/static/django_listing/css/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     9678 2020-07-23 13:29:12.000000 django-listing-0.5.0/django_listing/static/django_listing/css/dropzone.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16503 2020-05-04 16:11:45.000000 django-listing-0.5.0/django_listing/static/django_listing/css/jquery.datetimepicker.min.css
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    16264 2023-06-26 06:53:59.000000 django-listing-0.5.0/django_listing/static/django_listing/css/select2.min.css
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/static/django_listing/js/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11591 2023-06-25 15:39:35.000000 django-listing-0.5.0/django_listing/static/django_listing/js/django_listing.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6969 2023-06-26 10:45:52.000000 django-listing-0.5.0/django_listing/static/django_listing/js/django_listing.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    47430 2020-07-23 13:29:13.000000 django-listing-0.5.0/django_listing/static/django_listing/js/dropzone.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    60579 2020-05-04 16:11:45.000000 django-listing-0.5.0/django_listing/static/django_listing/js/jquery.datetimepicker.full.min.js
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    73163 2023-06-26 06:53:10.000000 django-listing-0.5.0/django_listing/static/django_listing/js/select2.min.js
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.711556 django-listing-0.5.0/django_listing/templates/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.711556 django-listing-0.5.0/django_listing/templates/django_listing/
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap4/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      181 2023-02-05 10:40:51.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap4/readme.txt
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1962 2023-06-19 06:34:04.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/filters_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      818 2023-02-05 16:44:01.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/tbi_dropdown.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1497 2023-02-05 16:44:01.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/tbi_select.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2023-02-05 16:44:01.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/tbi_update.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2023-02-05 16:44:01.000000 django-listing-0.5.0/django_listing/templates/django_listing/bootstrap5/tbi_variations.html
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/templates/django_listing/default/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1785 2020-08-13 07:02:47.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/action_footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      809 2023-04-28 23:01:05.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/action_header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1804 2023-07-05 09:51:43.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/actions_buttons.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        9 2018-05-13 07:49:23.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/div_row.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      226 2020-08-13 07:02:47.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/empty_listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1982 2023-06-25 12:24:47.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/filters_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2605 2023-06-26 07:46:14.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/footer.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1005 2023-06-26 07:38:04.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/header.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6677 2023-06-20 10:08:26.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/listing.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1175 2023-02-05 16:17:41.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/listing_div.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2759 2020-05-17 09:45:41.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/listing_form.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13292 2021-08-19 06:39:39.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/paginator.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      277 2019-04-09 10:09:14.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/selection_overlay.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      815 2023-02-02 17:30:06.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_dropdown.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1557 2020-05-19 13:04:19.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_select.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      384 2020-08-13 07:02:47.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_update.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      693 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_variations.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      202 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/toolbar.html
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1338 2023-06-21 16:08:14.000000 django-listing-0.5.0/django_listing/templates/django_listing/default/view_object_popup.html
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.723556 django-listing-0.5.0/django_listing/templatetags/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2018-04-20 16:44:23.000000 django-listing-0.5.0/django_listing/templatetags/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    12101 2023-06-23 14:56:54.000000 django-listing-0.5.0/django_listing/templatetags/django_listing.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     5197 2023-06-20 11:10:25.000000 django-listing-0.5.0/django_listing/theme_config.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    10288 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/toolbar.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2147 2023-04-27 22:59:09.000000 django-listing-0.5.0/django_listing/utils.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    18216 2023-06-26 15:53:38.000000 django-listing-0.5.0/django_listing/views.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-07-05 12:43:18.715556 django-listing-0.5.0/django_listing.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     6359 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    13420 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       55 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       15 2023-07-05 12:43:18.000000 django-listing-0.5.0/django_listing.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-07-05 12:43:18.727556 django-listing-0.5.0/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2138 2023-04-27 22:59:09.000000 django-listing-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-listing-0.0.9/django_listing.egg-info/PKG-INFO` & `django-listing-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,183 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.0.9
+Version: 0.5.0
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
-Description: 
-        ==============
-        django-listing
-        ==============
-        
-        .. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro1.png
-        .. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro2.png
-        
-        Django app for building HTML listings / tables, it includes many features :
-        
-        * Any iterable, Django QuerySet or model can be used.
-        * Most listings can be configured into a template file without touching a python file
-        * A class-based ListingView is provided if you want to code a listing at python side
-        * It as an Ajax mode to save requests to the server
-        * Uses JQuery if ajax is activated
-        * Customized for Bootstrap by default, but can be easily customized in many way (templates, icons, etc...)
-        * You can select columns to display, columns title, default sorting etc..
-        * Pagination is highly customizable (buttons to display, goto page, ellipsis, icons et labels)
-        * Rows can be <div> instead of <tr>, so it is possible to format data in many ways
-        * A lot of column types are provided, they are automatically created when a
-          QuerySet or a model is provided
-        * Columns are class-bases and one can create custom ones
-        * Columns manage One-to-many, Many-to-many and foreign relations
-        * Provides aggregation columns : sum, avg, min, max values
-        * Provides page-level and global aggregation : sum, avg, min, max values displayed at listing last row
-        * Provides columns to make a link to the object, a custom link, checkbox, select box, text input...
-        * Provides "action column" that comes with many actions : show, edit, delete, move up, move down...
-        * is able to manage multiple variations to present data in multiple way at the same place
-          (text only listing, text+image listing, image only listing for example)
-        * Uses Django translation framework : one can translate the listing as needed
-        * Toolbars can be added at the top and/or at the bottom to make actions
-        * Built-in toolbar action are : sorting, select a listing variation, number of rows per page,
-          export data. They are customizable.
-        * Toolbar items are class-based : one can create a custom one easily
-        * django-listing can automatically create a filter form (aka search form)
-        * Listing rows can be selectable in order to apply some actions
-        * Listings can be editable for mass updates
-        * django-listing can automatically create a form for inserting data to database
-        * One can upload files/images into a listing, it uses DropzoneJS (Work in progress)
-        * ListingView can manage itself database inserting, editing, deleting, filtering, uploads and actions :
-          no need to develop any code for that.
-        * django-listing comes with hundreds of icons as a scalable font
-        * django-listing is faster than django-table2
-        
-        
-        Demo
-        ----
-        
-        If you have docker you can run the demo with this command::
-        
-            docker run -p 8123:8123 elapouya/django-listing-demo
-        
-        And then open your browser at this url : http://localhost:8123
-        
-        To install docker on Linux, just use this command::
-        
-            curl -sSL https://get.docker.com/ | sh
-        
-        Otherwise, you can upload from here : https://docs.docker.com/get-docker/
-        
-        Code
-        ....
-        
-        The demo code is available on github here : `django-listing-demo <https://github.com/elapouya/django-listing-demo>`_
-        
-        
-        License
-        -------
-        Django-listing is licensed under the GPLv3 license for all open source applications.
-        A commercial license is required for all commercial applications or non-open applications
-        
-        See `LICENSE.rst <https://github.com/elapouya/django-listing/blob/master/LICENSE.rst>`_ file for more informations.
-        
-        
-        Documentation
-        -------------
-        
-        Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
-        
-        News
-        ----
-        
-        0.0.9 (2021-11-09)
-        ------------------
-        - Add possibility to create custom action button linked with listing method
-        
-        0.0.7 (2020-07-14)
-        ------------------
-        - First running version
-        
-        0.0.1 (2018-02-03)
-        ------------------
-        - Skeleton commit
-        
-        
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+License-File: LICENSE.rst
+
+
+==============
+django-listing
+==============
+
+.. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro1.png
+.. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro2.png
+
+Django app for building HTML listings / tables, it includes many features :
+
+* Any iterable, Django QuerySet or model can be used.
+* Most listings can be configured into a template file without touching a python file
+* A class-based ListingView is provided if you want to code a listing at python side
+* It as an Ajax mode to save requests to the server
+* Uses JQuery if ajax is activated
+* Customized for Bootstrap by default, but can be easily customized in many way (templates, icons, etc...)
+* You can select columns to display, columns title, default sorting etc..
+* Pagination is highly customizable (buttons to display, goto page, ellipsis, icons et labels)
+* Rows can be <div> instead of <tr>, so it is possible to format data in many ways
+* A lot of column types are provided, they are automatically created when a
+  QuerySet or a model is provided
+* Columns are class-bases and one can create custom ones
+* Columns manage One-to-many, Many-to-many and foreign relations
+* Provides aggregation columns : sum, avg, min, max values
+* Provides page-level and global aggregation : sum, avg, min, max values displayed at listing last row
+* Provides columns to make a link to the object, a custom link, checkbox, select box, text input...
+* Provides "action column" that comes with many actions : show, edit, delete, move up, move down...
+* is able to manage multiple variations to present data in multiple way at the same place
+  (text only listing, text+image listing, image only listing for example)
+* Uses Django translation framework : one can translate the listing as needed
+* Toolbars can be added at the top and/or at the bottom to make actions
+* Built-in toolbar action are : sorting, select a listing variation, number of rows per page,
+  export data. They are customizable.
+* Toolbar items are class-based : one can create a custom one easily
+* django-listing can automatically create a filter form (aka search form)
+* Listing rows can be selectable in order to apply some actions
+* Listings can be editable for mass updates
+* django-listing can automatically create a form for inserting data to database
+* One can upload files/images into a listing, it uses DropzoneJS (Work in progress)
+* ListingView can manage itself database inserting, editing, deleting, filtering, uploads and actions :
+  no need to develop any code for that.
+* django-listing comes with hundreds of icons as a scalable font
+* django-listing is faster than django-table2
+
+
+Showcase
+--------
+
+A demo is included in source code, you will need `poetry <https://python-poetry.org/docs/>`_ to install python environment::
+
+    curl -sSL https://install.python-poetry.org | python3 -
+
+To install the python envionment, go to django-listing source code root directory, then::
+
+    cd showcase
+    poetry install
+
+Check you are in ``showcase/`` directory, then start the Django from poetry environment::
+
+    poetry run python manage.py runserver 8123
+
+A sqlite database is already included, you do not have to make any migration,
+just open your brower at http://localhost:8123
+
+
+License
+-------
+Django-listing is licensed under the GPLv3 license for all open source applications.
+A commercial license is required for all commercial applications or non-open applications
+
+See `LICENSE.rst <https://github.com/elapouya/django-listing/blob/master/LICENSE.rst>`_ file for more informations.
+
+
+Documentation
+-------------
+
+Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
+
+News
+----
+
+0.5.0 (2023-07-05)
+------------------
+- Add __url_func parameter for edit/delete/view action buttons
+
+0.0.28 (2023-06-27)
+-------------------
+- Add AutocompleteMultipleForeignKeyFilter
+
+0.0.27 (2023-06-26)
+-------------------
+- Add ForeignKeyFilter and AutocompleteForeignKeyFilter
+
+0.0.26 (2023-06-21)
+-------------------
+- Added edit and delete action buttons
+- Fixed action button "see details" modal
+
+0.0.24 (2023-06-20)
+-------------------
+- Improved CSS for small device
+- Auto-detect many-to-many model fields if present in select_columns
+
+0.0.23 (2023-06-19)
+-------------------
+- Fixed choices widgets
+
+0.0.22 (2023-06-19)
+-------------------
+- Improved radio and checkbox in filter form
+
+0.0.21 (2023-06-15)
+-------------------
+- Fixed ModelColumns
+
+0.0.20 (2023-05-19)
+-------------------
+- Added LineNumberColumn()
+
+0.0.18 (2023-05-05)
+-------------------
+- Use scss to generate css files
+
+0.0.17 (2023-04-26)
+-------------------
+- Added showcase with many demo pages see showcase/README.rst
+
+0.0.14 (2022-10-24)
+-------------------
+- Fixed bad form closing
+- Fixed ListingVariation with Ajax
+
+0.0.12 (2022-07-04)
+-------------------
+- Added django-like filter syntax for sequences
+
+0.0.11 (2022-06-02)
+-------------------
+- Added JsonDateTimeColumn class
+
+0.0.10 (2022-05-17)
+-------------------
+- Added support for python 3.10
+
+0.0.9 (2021-11-09)
+------------------
+- Added possibility to create custom action button linked with listing method
+
+0.0.7 (2020-07-14)
+------------------
+- First running version
+
+0.0.1 (2018-02-03)
+------------------
+- Skeleton commit
+
```

### Comparing `django-listing-0.0.9/LICENSE.rst` & `django-listing-0.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/setup.py` & `django-listing-0.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,77 @@
-from setuptools import setup,find_packages
 import os
 import re
 
+from setuptools import find_packages, setup
+
 
 def read(*names):
     values = dict()
     for name in names:
-        filename = name + '.rst'
+        filename = name + ".rst"
         if os.path.isfile(filename):
             fd = open(filename)
             value = fd.read()
             fd.close()
         else:
-            value = ''
+            value = ""
         values[name] = value
     return values
 
 
 long_description = """
 %(README)s
 
 News
 ----
 
 %(CHANGES)s
-""" % read('README', 'CHANGES')
+""" % read(
+    "README", "CHANGES"
+)
 
 
 def get_version(pkg):
-    path = os.path.join(os.path.dirname(__file__), pkg, '__init__.py')
+    path = os.path.join(os.path.dirname(__file__), pkg, "__init__.py")
     with open(path) as fh:
         m = re.search(r'^__version__\s*=\s*[\'"]([^\'"]+)[\'"]', fh.read(), re.M)
     if m:
         return m.group(1)
     raise RuntimeError("Unable to find __version__ string in %s." % path)
 
-print(find_packages(exclude=['docs.*','docs']))
 
-setup(name='django-listing',
-      version=get_version('django_listing'),
-      description='Library for creating HTML listing / table / data grid',
-      long_description=long_description,
-      classifiers=[
-          "Intended Audience :: Developers",
-          "Development Status :: 3 - Alpha",
-          "Framework :: Django",
-          "Framework :: Django :: 2.0",
-          "Framework :: Django :: 3.0",
-          "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-          "Programming Language :: Python",
-          "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.6",
-      ],
-      keywords='table, datatable, listing, data grid',
-      url='https://github.com/elapouya/django-listing',
-      author='Eric Lapouyade',
-      author_email='elapouya@gmail.com',
-      license='GPLv3+',
-      packages=find_packages(exclude=['docs.*','docs']),
-      include_package_data=True,
-      install_requires=['django>=2', 'tablib'],
-      extras_require={
-        'docs': ['Sphinx', 'sphinxcontrib-napoleon'],
-      },
-      zip_safe=False)
+# print(find_packages(exclude=['showcase', 'docs']))
+
+setup(
+    name="django-listing",
+    version=get_version("django_listing"),
+    description="Library for creating HTML listing / table / data grid",
+    long_description=long_description,
+    classifiers=[
+        "Intended Audience :: Developers",
+        "Development Status :: 3 - Alpha",
+        "Framework :: Django",
+        "Framework :: Django :: 2.0",
+        "Framework :: Django :: 3.0",
+        "Framework :: Django :: 4.0",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    keywords="table, datatable, listing, data grid",
+    url="https://github.com/elapouya/django-listing",
+    author="Eric Lapouyade",
+    author_email="elapouya@gmail.com",
+    license="GPLv3+",
+    packages=find_packages(exclude=["showcase", "docs"]),
+    include_package_data=True,
+    install_requires=["django>=2", "tablib"],
+    extras_require={
+        "docs": ["Sphinx", "sphinxcontrib-napoleon"],
+    },
+    zip_safe=False,
+)
```

### Comparing `django-listing-0.0.9/django_listing/record.py` & `django-listing-0.5.0/django_listing/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,98 @@
 #
 # Created : 2018-02-09
 #
 # @author: Eric Lapouyade
 #
 
 import collections
-from .exceptions import *
+import os
+import re
+import types
+from urllib.parse import quote_plus
+
+from django.db import models
+from django.db.models import F, Model
 from django.db.models.query import QuerySet
-from django.db.models import F
 from django.utils.safestring import mark_safe
-from django.db import models
-from django.utils.translation import ugettext as _
-from urllib.parse import quote_plus
-import types
-import re
-import os
+from django.utils.translation import gettext as _
+
+from .exceptions import *
 
-__all__ = ['RecordManager', 'Record', 'cache_in_record']
+__all__ = ["RecordManager", "Record", "cache_in_record"]
 
 
 def cache_in_record(value_func):
     def cached_value_func(self, rec):
         cached, value = rec.get_cached_cell_value(self)
         if not cached:
             value = value_func(self, rec)
             rec.set_cached_cell_value(self, value)
         return value
+
     return cached_value_func
 
 
 class SequenceItem:
     def __init__(self, pk, obj):
         self.pk = pk
         self.obj = obj
 
 
 # Records are always bound to a listing instance
 class RecordManager:
-    def __init__(self,listing):
+    def __init__(self, listing):
         self.listing = listing
         self._records = None
 
     def get_all(self):
         # used only for sequences (and short sequences please !)
         lsg = self.listing
-        if isinstance(lsg.data,QuerySet):
-            raise InvalidListing(_('Getting all records is only supported on '
-                                   'SMALL sequence data, not on Django querysets'))
-        if not hasattr(lsg, '_all_records'):
-            lsg._all_records = [ Record(lsg, rec, i)
-                                 for i,rec in enumerate(lsg.data) ]
+        if isinstance(lsg.data, QuerySet):
+            raise InvalidListing(
+                _(
+                    "Getting all records is only supported on "
+                    "SMALL sequence data, not on Django querysets"
+                )
+            )
+        if not hasattr(lsg, "_all_records"):
+            lsg._all_records = [Record(lsg, rec, i) for i, rec in enumerate(lsg.data)]
         return lsg._all_records
 
     def get_first_obj(self):
-        if not hasattr(self,'_first_obj'):
+        if not hasattr(self, "_first_obj"):
             qs = self.get_objs_from_queryset()
             self._first_obj = qs.first()
         return self._first_obj
 
     def get_last_obj(self):
-        if not hasattr(self,'_last_obj'):
+        if not hasattr(self, "_last_obj"):
             qs = self.get_objs_from_queryset()
             self._last_obj = qs.last()
         return self._last_obj
 
     def clear_first_last_cache(self):
-        if hasattr(self, '_first_obj'):
-            delattr(self, '_first_obj')
-        if hasattr(self, '_last_obj'):
-            delattr(self, '_last_obj')
+        if hasattr(self, "_first_obj"):
+            delattr(self, "_first_obj")
+        if hasattr(self, "_last_obj"):
+            delattr(self, "_last_obj")
 
     def get_obj(self, **kwargs):
         lsg = self.listing
         if isinstance(lsg.data, QuerySet):
             qs = self.get_objs_from_queryset()
             try:
                 return qs.get(**kwargs)
             except qs.DoesNotExist:
                 return None
         else:
             # actually work only with 'id' or 'pk'
-            pk = kwargs.get('pk')
+            pk = kwargs.get("pk")
             if pk is None:
-                pk = kwargs.get('id')
+                pk = kwargs.get("id")
             if pk is None:
                 return None
             return self.get_objs_from_sequence()[pk].obj
 
     def get_rec(self, **kwargs):
         obj = self.get_obj(**kwargs)
         if obj is None:
@@ -94,97 +100,102 @@
         return Record(self.listing, obj)
 
     def move_obj_order(self, obj, field, delta):
         qs = self.get_objs_from_queryset()
         obj_order = getattr(obj, field)
         if not isinstance(obj_order, int):
             raise ListingException(
-                _('field "{field}" must be an integer, please choose the '
-                  'correct field that will be used to change object ordering')
-                  .format(field=field))
+                _(
+                    'field "{field}" must be an integer, please choose the '
+                    "correct field that will be used to change object ordering"
+                ).format(field=field)
+            )
         new_order = obj_order + delta
         if delta < 0:
-            qs = qs.filter(**{ f'{field}__gte':new_order,
-                               f'{field}__lt':obj_order } )
-            qs.update(**{field:F(field)+1})
+            qs = qs.filter(**{f"{field}__gte": new_order, f"{field}__lt": obj_order})
+            qs.update(**{field: F(field) + 1})
             setattr(obj, field, new_order)
             obj.save()
             self.clear_first_last_cache()
         elif delta > 0:
-            qs = qs.filter(**{ f'{field}__gt':obj_order,
-                               f'{field}__lte':new_order } )
-            qs.update(**{field:F(field)-1})
+            qs = qs.filter(**{f"{field}__gt": obj_order, f"{field}__lte": new_order})
+            qs.update(**{field: F(field) - 1})
             setattr(obj, field, new_order)
             obj.save()
             self.clear_first_last_cache()
 
     def compute_current_page_records(self):
         lsg = self.listing
-        if not isinstance(lsg.data,(collections.Sequence,QuerySet)):
-            raise InvalidData(_('Listing data must be a sequence or a QuerySet.'))
-        if isinstance(lsg.data,QuerySet):
+        if not isinstance(lsg.data, (collections.abc.Sequence, QuerySet)):
+            raise InvalidData(_("Listing data must be a sequence or a QuerySet."))
+        if isinstance(lsg.data, QuerySet):
             objs = self.get_objs_from_queryset()
         else:
             objs = self.get_objs_from_sequence()
 
         per_page = int(lsg.per_page)
         if per_page <= 0 or per_page > lsg.per_page_max:
             per_page = lsg.per_page_max
         lsg.paginator = lsg.paginator_class(
-            lsg, objs, per_page,
-            lsg.orphans,lsg.allow_empty_first_page)
+            lsg, objs, per_page, lsg.orphans, lsg.allow_empty_first_page
+        )
         lsg.current_page = lsg.paginator.get_page(lsg.page or 1)
         if lsg.editable and lsg.editing:
             self.bind_formset()
 
     def current_page(self):
         if not self._records:
             lsg = self.listing
-            self._records = [ Record(lsg,obj,i)
-                              for i,obj in enumerate(lsg.current_page) ]
+            self._records = [
+                Record(lsg, obj, i) for i, obj in enumerate(lsg.current_page)
+            ]
         return self._records
 
     def bind_formset(self):
         if self.listing.editing_row_pk:
             formset = self.listing.get_formset()
             for rec in self.current_page():
                 if rec.pk == self.listing.editing_row_pk:
                     rec.set_form(formset[0])
         else:
-            for rec, form in zip(self.current_page(),self.listing.get_formset()):
+            for rec, form in zip(self.current_page(), self.listing.get_formset()):
                 rec.set_form(form)
 
     def export(self):
         lsg = self.listing
-        for i,obj in enumerate(lsg.data):
-            yield Record(self.listing,obj,i)
+        for i, obj in enumerate(lsg.data):
+            yield Record(self.listing, obj, i)
 
     def filter_queryset(self, qs):
         if self.listing.filters:
             form = self.listing.filters.form()
             if form.is_valid():
                 for filtr in self.listing.filters:
                     qs = filtr.filter_queryset(qs, form.cleaned_data)
         return qs
 
     def get_objs_from_queryset(self):
-        if not hasattr(self, '_queryset_objs'):
+        if not hasattr(self, "_queryset_objs"):
             lsg = self.listing
             qs = self.listing.data
             qs = self.filter_queryset(qs)
             order_by = []
             if lsg.sort:
                 for col_name in lsg.columns_sort_list:
-                    order_prefix = '' if lsg.columns_sort_ascending[col_name] else '-'
+                    order_prefix = "" if lsg.columns_sort_ascending[col_name] else "-"
                     col = lsg.columns.get(col_name)
                     if col:
-                        order_by.append(order_prefix + col.sort_key)
+                        if isinstance(col.sort_key, (tuple, list)):
+                            for sort_key in col.sort_key:
+                                order_by.append(order_prefix + sort_key)
+                        else:
+                            order_by.append(order_prefix + col.sort_key)
             # add a default sorting to avoid a Django 'UnorderedObjectListWarning'
             if not order_by:
-                order_by = ['pk']
+                order_by = ["pk"]
             self._queryset_objs = qs.order_by(*order_by)
         return self._queryset_objs
 
     def filter_sequence(self, seq):
         if self.listing.filters:
             for filtr in self.listing.filters:
                 seq = filtr.filter_sequence(seq)
@@ -198,19 +209,25 @@
             for col_name in reversed(lsg.columns_sort_list):
                 col = lsg.columns.get(col_name)
                 if col:
                     sort_key = col.sort_key
                     if callable(sort_key):
                         key_func = sort_key
                     else:
+
                         def key_func(rec):
                             return rec[sort_key]
-                    seq = sorted(seq,key=key_func,
-                                 reverse=not lsg.columns_sort_ascending[col_name])
-        return [ SequenceItem(i,obj) for i,obj in enumerate(seq) ]
+
+                    seq = sorted(
+                        seq,
+                        key=key_func,
+                        reverse=not lsg.columns_sort_ascending[col_name],
+                    )
+        return [SequenceItem(i, obj) for i, obj in enumerate(seq)]
+
 
 class Record:
     def __init__(self, listing, obj, index=0, form=None):
         self._listing = listing
         if isinstance(obj, SequenceItem):
             self._obj = obj.obj
             self.pk = obj.pk
@@ -219,16 +236,17 @@
         self._index = index
         self._cell_values = {}
         self._form = form
         self._selected = False
         if isinstance(self._obj, dict):
             self._format_ctx = self._obj
         elif isinstance(self._obj, (tuple, list)):
-            self._format_ctx = {self._listing.columns[i].name: val
-                                for i, val in enumerate(self._obj)}
+            self._format_ctx = {
+                self._listing.columns[i].name: val for i, val in enumerate(self._obj)
+            }
         else:
             self._format_ctx = vars(self._obj)
 
     def get_object(self):
         return self._obj
 
     def is_selected(self):
@@ -250,74 +268,86 @@
 
     def set_cached_cell_value(self, col, value):
         self._cell_values[col] = value
 
     def get_format_ctx(self):
         return self._format_ctx
 
-    def format_str(self, str_to_format):
-        return str_to_format.format(**self._format_ctx)
+    def format_str(self, str_to_format, extra_context=None):
+        context = {**self._format_ctx}
+        obj = self.get_object()
+        context.update(rec_object=obj)
+        if hasattr(obj, "get_absolute_url"):
+            context.update(rec_object_url=obj.get_absolute_url())
+        return mark_safe(str_to_format.format(**context))
 
     def get_listing(self):
         return self._listing
 
     def get_index(self):
         return self._index
 
     def get_filter(self, obj, filter_name, params):
-        if filter_name == 'urlencode' and isinstance(obj, str):
+        if filter_name == "urlencode" and isinstance(obj, str):
             obj = quote_plus(obj)
-        elif filter_name == 'replace':
+        elif filter_name == "replace":
             obj = obj.replace(*params)
-        elif filter_name == 'sub':
+        elif filter_name == "sub":
             obj = re.sub(*params, obj)
-        elif filter_name == 'basename':
+        elif filter_name == "basename":
             obj = os.path.basename(obj)
         else:
-            func = getattr(obj,filter_name,None)
+            func = getattr(obj, filter_name, None)
             if func is not None:
                 obj = func()
         return obj
 
     def get_href(self):
-        return self._obj.get_absolute_url()
+        if hasattr(self._obj, "get_absolute_url"):
+            return self._obj.get_absolute_url()
 
     def get(self, key, default=None):
         obj = self._obj
         try:
-            if isinstance(key,int):
+            if isinstance(key, int):
                 obj = obj[key]
             else:
-                key, *filter = key.split('|',1)
-                for subkey in key.split('.'):
+                key, *filter = key.split("|", 1)
+                for subkey in re.split(r"\.|__", key):
                     op = None
-                    if '|' in subkey:
-                        subkey, op = subkey.split('|')
+                    if "|" in subkey:
+                        subkey, op = subkey.split("|")
                     if subkey.isdigit():
                         obj = obj[int(subkey)]
                     else:
-                        if isinstance(obj,dict):
+                        if isinstance(obj, dict):
                             obj = obj[subkey]
                         else:
                             obj = getattr(obj, subkey)
-                    if isinstance(obj,types.MethodType):
+                    if isinstance(obj, types.MethodType):
                         obj = obj()
                 if obj is not None and filter:
                     filter = filter[0]
-                    filter_name, *params = filter.split(':')
-                    params = tuple(map(lambda s:s.replace('__C__',':'), params))
+                    filter_name, *params = re.split(r"(?<!\\):", filter)
+                    params = tuple(map(lambda s: re.sub(r"\\:", ":", s), params))
                     obj = self.get_filter(obj, filter_name, params)
-        except (IndexError, AttributeError, TypeError, KeyError):
+        except (
+            IndexError,
+            AttributeError,
+            TypeError,
+            KeyError,
+            models.ObjectDoesNotExist,
+        ):
             return default
         return obj
 
     def _digest(self):
-        out = ''
+        out = ""
         for c in self._listing.columns:
-            out += '<b>{} :</b> {}<br>\n'.format(c.name,c.get_cell_value(self))
+            out += "<b>{} :</b> {}<br>\n".format(c.name, c.get_cell_value(self))
         return out
 
     def __str__(self):
         return mark_safe(self._digest())
 
     def __getattr__(self, item):
         return self.get(item)
```

### Comparing `django-listing-0.0.9/django_listing/templatetags/django_listing.py` & `django-listing-0.5.0/django_listing/templatetags/django_listing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,188 +1,198 @@
-'''
+"""
 Création : 12 janv. 2010
 
 @author: Eric Lapouyade
-'''
+"""
+import json
+from itertools import count
+
 from django import template
 from django.conf import settings
-from django.utils.safestring import mark_safe, SafeString
+from django.utils.safestring import SafeString, mark_safe
+
 from ..listing import Listing, ListingVariations
 from ..listing_form import ListingForm
-from itertools import count
-from ..app_settings import app_settings
-from ..utils import JsonDirect
-import json
+from ..theme_config import ThemeTemplate
 
 register = template.Library()
 _uniq_counter = count(0)
 
 
-@register.filter(name='json_options')
+@register.filter(name="json_options")
 def json_options(dct):
-    out = '{\n'
+    out = "{\n"
     options = []
-    for k,v in sorted(dct.items()):
+    for k, v in sorted(dct.items()):
         if isinstance(v, SafeString):
-            options.append(f'{k}:{v}')
+            options.append(f"{k}:{v}")
         else:
-            options.append(f'{k}:{json.dumps(v, indent=4)}')
-    out += ',\n'.join(options)
-    out += '\n}'
+            options.append(f"{k}:{json.dumps(v, indent=4)}")
+    out += ",\n".join(options)
+    out += "\n}"
     return mark_safe(out)
 
 
 @register.filter()
 def underscore_to_dash(s):
-    return s.replace('_','-')
+    return s.replace("_", "-")
+
+
+@register.filter()
+def theme_template(s):
+    return ThemeTemplate.get(s)
 
 
 class ListingHeaderNode(template.Node):
     def __init__(self, nodelist):
         self.nodelist = nodelist
 
     def render(self, context):
         remaining_output = self.nodelist.render(context)
-        tpl = template.loader.get_template(app_settings.HEADER_TEMPLATE)
+        template_name = ThemeTemplate.get("header.html")
+        tpl = template.loader.get_template(template_name)
         request = context.request
         context = context.flatten()
         context.update(
-            app_settings.context,
-            need_media_for=getattr(context['request'], 'need_media_for',{})
+            settings.django_listing_settings.context,
+            need_media_for=getattr(context["request"], "need_media_for", {}),
         )
         tpl_output = tpl.render(context, request)
-        return f'{tpl_output}\n{remaining_output}'
+        return f"{tpl_output}\n{remaining_output}"
 
 
 @register.tag(name="render_listing_header")
 def do_listing_header(parser, token):
     nodelist = parser.parse()
     return ListingHeaderNode(nodelist)
 
 
 @register.simple_tag(takes_context=True)
 def render_listing_footer(context):
-    tpl = template.loader.get_template(app_settings.FOOTER_TEMPLATE)
+    template_name = ThemeTemplate.get("footer.html")
+    tpl = template.loader.get_template(template_name)
     request = context.request
     context = context.flatten()
     context.update(
-        app_settings.context,
-        need_media_for=getattr(context['request'],'need_media_for',{})
+        settings.django_listing_settings.context,
+        need_media_for=getattr(context["request"], "need_media_for", {}),
     )
     tpl_output = tpl.render(context, request)
     return tpl_output
 
 
 def initialize_listing(context, listing, data=None, *args, **kwargs):
-    if isinstance(listing,str) or listing is None:
+    if isinstance(listing, str) or listing is None:
         return None
-    if not isinstance(listing,(Listing,ListingVariations)):
+    if not isinstance(listing, (Listing, ListingVariations)):
         data = listing
         listing = Listing()
     # if there is data or a model is specified in columns (if exsiting)
-    if (data or listing.get_model()) and not listing.is_initialized():
+    if (data is not None or listing.get_model()) and not listing.is_initialized():
         listing.init(data, context=context, **kwargs)
     else:
         listing.set_kwargs(**kwargs)
     return listing
 
 
 @register.simple_tag(takes_context=True)
 def create_listing_begin(context, listing=None, *args, **kwargs):
     # developper will specify a Listing class,
     # but Django will automatically instanciate it with no argument
-    if not isinstance(listing,(Listing,ListingVariations)):
+    if not isinstance(listing, (Listing, ListingVariations)):
         listing = Listing()
     listing.store_kwargs(**kwargs)
     return listing
 
 
 @register.simple_tag(takes_context=True)
 def create_listing_end(context, listing, data=None, *args, **kwargs):
     initialize_listing(context, listing, data, *args, **kwargs)
-    return ''
+    return ""
 
 
 @register.simple_tag(takes_context=True)
 def create_listing(context, listing, data=None, *args, **kwargs):
     return initialize_listing(context, listing, data, *args, **kwargs)
 
 
 @register.simple_tag()
 def setopt_listing(listing, **kwargs):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_kwargs(**kwargs)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_listing_html_attr(listing, listing_attr, html_attr, value):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_html_attr(listing_attr, html_attr, value)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_column(listing, name, **kwargs):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_column_kwargs(name, **kwargs)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_column_html_attr(listing, name, col_attr, html_attr, value):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_column_html_attr(name, col_attr, html_attr, value)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_toolbar_item(listing, name, **kwargs):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_toolbar_item_kwargs(name, **kwargs)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_toolbar_item_html_attr(listing, name, col_attr, html_attr, value):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_toolbar_item_html_attr(name, col_attr, html_attr, value)
-    return ''
+    return ""
 
 
 @register.simple_tag(takes_context=True)
 def render_listing(context, listing=None, data=None, *args, **kwargs):
     if listing is None:
-        listing = context.get('listing')
+        listing = context.get("listing")
     listing = initialize_listing(context, listing, data, *args, **kwargs)
     if listing is None:
         return mark_safe(
-                '<b>ERROR :</b> The listing/class/data you specified is '
-                'empty : do you have set the corresponding variable '
-                'in view context ?')
-    if isinstance(listing.data,str) or listing.data is None:
+            "<b>ERROR :</b> The listing/class/data you specified is "
+            "empty : do you have set the corresponding variable "
+            "in view context ?"
+        )
+    if isinstance(listing.data, str) or listing.data is None:
         return mark_safe(
-                '<b>ERROR :</b> The listing has no data or model specified : '
-                'May be you passed a listing class and forgot to specify data '
-                'or model or you passed only a listing instance but without any'
-                ' bound data. Please check you have '
-                '<tt>{% render_listing your_listing_class_or_instance your_data'
-                ' %}</tt> or specify data or a django model when creating '
-                'the listing class or instance in your python code.')
+            "<b>ERROR :</b> The listing has no data or model specified : "
+            "May be you passed a listing class and forgot to specify data "
+            "or model or you passed only a listing instance but without any"
+            " bound data. Please check you have "
+            "<tt>{% render_listing your_listing_class_or_instance your_data"
+            " %}</tt> or specify data or a django model when creating "
+            "the listing class or instance in your python code."
+        )
     return mark_safe(listing.render(context))
 
 
 @register.simple_tag(takes_context=True)
 def geturl_listing(context, listing, **kwargs):
     return mark_safe(listing.get_url(context, **kwargs))
 
 
 @register.simple_tag(takes_context=True)
 def geturl_listing_key(context, listing, key, value, **kwargs):
-    return mark_safe(listing.get_url(context, **{key:value}, **kwargs))
+    return mark_safe(listing.get_url(context, **{key: value}, **kwargs))
 
 
 @register.simple_tag()
 def gethiddens_listing(listing, without=None):
     return mark_safe(listing.get_hiddens_html(without))
 
 
@@ -195,134 +205,163 @@
 def get_uniq_id():
     return next(_uniq_counter)
 
 
 @register.simple_tag(takes_context=True)
 def render_filters_form(context, listing):
     if not listing:
-        listing = context.get('listing')
+        listing = context.get("listing")
     listing = initialize_listing(context, listing)
     if not listing or not listing.is_initialized():
         return mark_safe(
-            '<b>ERROR :</b> The listing must be initialized before rendering the'
-            ' filter form. You should use <tt>{% create_listing a_listing_class '
-            'your_data as listing %}</tt> tag before in '
-            'the template or provide in the context a listing instance bound '
-            'to some data.<br><br>')
-    if not isinstance(listing,(Listing,ListingVariations)):
+            "<b>ERROR :</b> The listing must be initialized before rendering the"
+            " filter form. You should use <tt>{% create_listing a_listing_class "
+            "your_data as listing %}</tt> tag before in "
+            "the template or provide in the context a listing instance bound "
+            "to some data.<br><br>"
+        )
+    if not isinstance(listing, (Listing, ListingVariations)):
         return mark_safe(
-            '<b>ERROR :</b> You specified an invalid listing instance. '
-            'Do you have set the corresponding variable in view context ?')
+            "<b>ERROR :</b> You specified an invalid listing instance. "
+            "Do you have set the corresponding variable in view context ?"
+        )
     if not listing.filters:
         return mark_safe(
-            '<b>ERROR :</b> The listing has no filters defined. '
+            "<b>ERROR :</b> The listing has no filters defined. "
             'Please define the ".filters" attribute to your listing'
-            )
+        )
     return mark_safe(listing.filters.render_form(context))
 
 
 @register.simple_tag()
 def setopt_filter(listing, name, **kwargs):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_filter_kwargs(name, **kwargs)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def setopt_filter_html_attr(listing, name, col_attr, html_attr, value):
-    if isinstance(listing,(Listing,ListingVariations)):
+    if isinstance(listing, (Listing, ListingVariations)):
         listing.store_filter_html_attr(name, col_attr, html_attr, value)
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def filters_form_field(listing, name):
     return listing.filters.get_form_field(name)
 
 
 @register.simple_tag()
+def filters_form_field_container_attrs(listing, name):
+    return mark_safe(listing.filters.get_form_field_container_attrs(name))
+
+
+@register.simple_tag()
 def filters_add_row(listing, row):
     if listing.filters is None:
         listing.filters = row
-    elif isinstance(listing.filters,str):
+    elif isinstance(listing.filters, str):
         if listing.filters:
-            listing.filters += ';'
+            listing.filters += ";"
         listing.filters += row
-    return ''
+    return ""
 
 
 @register.simple_tag()
 def get_form_field(form, name):
     return form[name]
 
 
 @register.simple_tag(takes_context=True)
-def render_listing_form(context, listing, *args,
-                        action=None, layout=None, name=None, **kwargs):
+def render_listing_form(
+    context, listing, *args, action=None, layout=None, name=None, **kwargs
+):
     if not listing:
-        listing = context.get('listing')
-    if not isinstance(listing,(Listing,ListingVariations)):
+        listing = context.get("listing")
+    if not isinstance(listing, (Listing, ListingVariations)):
         return mark_safe(
-            '<b>ERROR :</b> You specified an invalid listing instance. '
-            'Do you have set the corresponding variable in view context ?')
+            "<b>ERROR :</b> You specified an invalid listing instance. "
+            "Do you have set the corresponding variable in view context ?"
+        )
     if listing.form:
         if not isinstance(listing.form, ListingForm):
             return mark_safe(
-                '<b>ERROR :</b> when using {% render_listing_form listing %}'
-                'listing.form must be an instance of ListingForm')
+                "<b>ERROR :</b> when using {% render_listing_form listing %}"
+                "listing.form must be an instance of ListingForm"
+            )
         if layout:
             if listing.form.layout:
                 return mark_safe(
-                    '<b>ERROR :</b> Do not specify a layout in '
-                    '{% render_listing_form %} when a layout has already been  '
-                    'defined at python side.<br><br>')
+                    "<b>ERROR :</b> Do not specify a layout in "
+                    "{% render_listing_form %} when a layout has already been  "
+                    "defined at python side.<br><br>"
+                )
             else:
                 listing.form.layout = layout
         if action:
             if listing.form.action:
                 return mark_safe(
-                    '<b>ERROR :</b> Do not specify an action in '
-                    '{% render_listing_form %} when an action has already been  '
-                    'defined at python side.<br><br>')
+                    "<b>ERROR :</b> Do not specify an action in "
+                    "{% render_listing_form %} when an action has already been  "
+                    "defined at python side.<br><br>"
+                )
             else:
                 listing.form.action = action
     if not listing.form:
-        listing.form = ListingForm(action, name=name,
-                                   layout=layout, *args, **kwargs)
+        listing.form = ListingForm(action, name=name, layout=layout, *args, **kwargs)
     listing.form.bind_to_listing(listing)
     return mark_safe(listing.form.render(context))
 
 
 @register.simple_tag(takes_context=True)
 def get_dict_list(context, key):
     request = context.request
-    if hasattr(request, 'django_listing_footer_dict_list'):
+    if hasattr(request, "django_listing_footer_dict_list"):
         return request.django_listing_footer_dict_list.get(key, [])
     return []
 
 
 @register.simple_tag(takes_context=True)
 def header_snippets(context):
     request = context.request
-    snippets = getattr(request, 'django_listing_header_snippets', None)
+    snippets = getattr(request, "django_listing_header_snippets", None)
     if snippets:
-        return mark_safe('\n'.join(snippets))
-    return ''
+        return mark_safe("\n".join(snippets))
+    return ""
 
 
 @register.simple_tag(takes_context=True)
 def footer_snippets(context):
     request = context.request
-    snippets = getattr(request, 'django_listing_footer_snippets', None)
+    snippets = getattr(request, "django_listing_footer_snippets", None)
     if snippets:
-        return mark_safe('\n'.join(snippets))
-    return ''
+        return mark_safe("\n".join(snippets))
+    return ""
 
 
 @register.simple_tag(takes_context=True)
 def onready_snippets(context):
     request = context.request
-    snippets = getattr(request, 'django_listing_onready_snippets', None)
+    snippets = getattr(request, "django_listing_onready_snippets", None)
     if snippets:
-        return mark_safe('\n'.join(snippets))
-    return ''
+        return mark_safe("\n".join(snippets))
+    return ""
+
 
+@register.simple_tag()
+def listing_responsive_columns_css(listing, format_str=None):
+    if not isinstance(listing, (Listing, ListingVariations)):
+        return mark_safe(
+            "<!-- ERROR : you must provide a valid listing to {% listing_responsive_css %} -->"
+        )
+    css = []
+    if format_str is None:
+        format_str = "{} : "
+    for i, col in enumerate(listing.selected_columns, start=1):
+        title = col.get_header_value()
+        content = format_str.format(title, col=col)
+        css_class = listing.theme_listing_class.replace(" ", ".")
+        css.append(
+            f"table.{css_class} td:nth-of-type({i}):before {{content: '{content}';}}"
+        )
+    return mark_safe("\n".join(css))
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/paginator.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/paginator.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/tbi_dropdown.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_dropdown.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/listing_form.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/listing_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/tbi_variations.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_variations.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/action_footer.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/action_footer.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/listing.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/listing.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,395 +1,418 @@
 00000000: 7b25 206c 6f61 6420 646a 616e 676f 5f6c  {% load django_l
 00000010: 6973 7469 6e67 2025 7d0a 7b25 2061 7574  isting %}.{% aut
 00000020: 6f65 7363 6170 6520 6f66 6620 257d 0a20  oescape off %}. 
 00000030: 2020 203c 6469 7620 6964 3d22 7b7b 206c     <div id="{{ l
-00000040: 6973 7469 6e67 2e69 647c 756e 6465 7273  isting.id|unders
-00000050: 636f 7265 5f74 6f5f 6461 7368 207d 7d22  core_to_dash }}"
-00000060: 0a20 2020 2020 2020 2020 6c69 7374 696e  .         listin
-00000070: 672d 7375 6666 6978 3d22 7b7b 206c 6973  g-suffix="{{ lis
-00000080: 7469 6e67 2e73 7566 6669 7820 7d7d 220a  ting.suffix }}".
-00000090: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-000000a0: 7b7b 206c 6973 7469 6e67 5f63 6f6e 7461  {{ listing_conta
-000000b0: 696e 6572 5f63 6c61 7373 207d 7d22 0a20  iner_class }}". 
-000000c0: 2020 2020 2020 2020 616a 6178 5f75 726c          ajax_url
-000000d0: 3d22 7b7b 206c 6973 7469 6e67 2e67 6574  ="{{ listing.get
-000000e0: 5f75 726c 207d 7d22 0a20 2020 2020 2020  _url }}".       
-000000f0: 2020 7b25 2069 6620 6c69 7374 696e 672e    {% if listing.
-00000100: 7365 6c65 6374 696f 6e5f 6d65 6e75 5f69  selection_menu_i
-00000110: 6420 257d 7365 6c65 6374 696f 6e2d 6d65  d %}selection-me
-00000120: 6e75 2d69 643d 227b 7b20 6c69 7374 696e  nu-id="{{ listin
-00000130: 672e 7365 6c65 6374 696f 6e5f 6d65 6e75  g.selection_menu
-00000140: 5f69 6420 7d7d 227b 2520 656e 6469 6620  _id }}"{% endif 
-00000150: 257d 0a20 2020 203e 0a20 2020 203c 6469  %}.    >.    <di
-00000160: 7620 636c 6173 733d 226c 6973 7469 6e67  v class="listing
-00000170: 2d73 7069 6e6e 6572 223e 3c73 7061 6e20  -spinner"><span 
-00000180: 636c 6173 733d 227b 7b20 6c69 7374 696e  class="{{ listin
-00000190: 672e 7468 656d 655f 7370 696e 6e65 725f  g.theme_spinner_
-000001a0: 6963 6f6e 207d 7d22 3e3c 2f73 7061 6e3e  icon }}"></span>
-000001b0: 3c2f 6469 763e 0a0a 2020 2020 2020 2020  </div>..        
-000001c0: 7b25 2069 6620 6c69 7374 696e 672e 726f  {% if listing.ro
-000001d0: 775f 666f 726d 5f65 7272 6f72 7320 257d  w_form_errors %}
-000001e0: 0a20 2020 2020 2020 2020 2020 203c 756c  .            <ul
-000001f0: 2063 6c61 7373 3d22 6c69 7374 696e 672d   class="listing-
-00000200: 726f 772d 666f 726d 2d65 7272 6f72 7322  row-form-errors"
-00000210: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000220: 2020 7b25 2066 6f72 2065 7272 6f72 2069    {% for error i
-00000230: 6e20 6c69 7374 696e 672e 726f 775f 666f  n listing.row_fo
-00000240: 726d 5f65 7272 6f72 7320 257d 3c6c 693e  rm_errors %}<li>
-00000250: 7b7b 6572 726f 727c 7361 6665 7d7d 3c2f  {{error|safe}}</
-00000260: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
-00000270: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-00000280: 0a20 2020 2020 2020 2020 2020 203c 2f75  .            </u
-00000290: 6c3e 0a20 2020 2020 2020 207b 2520 656e  l>.        {% en
-000002a0: 6469 6620 257d 0a0a 2020 2020 2020 2020  dif %}..        
-000002b0: 7b25 2069 6620 6c69 7374 696e 672e 7061  {% if listing.pa
-000002c0: 6769 6e61 746f 722e 636f 756e 7420 6f72  ginator.count or
-000002d0: 206e 6f74 206c 6973 7469 6e67 2e65 6d70   not listing.emp
-000002e0: 7479 5f6c 6973 7469 6e67 5f74 656d 706c  ty_listing_templ
-000002f0: 6174 655f 6e61 6d65 2025 7d0a 2020 2020  ate_name %}.    
-00000300: 2020 2020 2020 2020 7b25 2069 6620 6861          {% if ha
-00000310: 735f 746f 705f 746f 6f6c 6261 7220 257d  s_top_toolbar %}
-00000320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000330: 203c 6469 7620 636c 6173 733d 2274 6f70   <div class="top
-00000340: 2d74 6f6f 6c62 6172 223e 0a20 2020 2020  -toolbar">.     
-00000350: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000360: 2520 696e 636c 7564 6520 6c69 7374 696e  % include listin
-00000370: 672e 746f 6f6c 6261 722e 7465 6d70 6c61  g.toolbar.templa
-00000380: 7465 5f6e 616d 6520 257d 0a20 2020 2020  te_name %}.     
-00000390: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-000003a0: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-000003b0: 2065 6e64 6966 2025 7d0a 0a20 2020 2020   endif %}..     
-000003c0: 2020 2020 2020 207b 2520 6966 206c 6973         {% if lis
-000003d0: 7469 6e67 2e63 616e 5f65 6469 7420 6f72  ting.can_edit or
-000003e0: 206c 6973 7469 6e67 2e68 6173 5f75 706c   listing.has_upl
-000003f0: 6f61 6420 6f72 206c 6973 7469 6e67 2e65  oad or listing.e
-00000400: 6469 745f 6f6e 5f64 656d 616e 6420 257d  dit_on_demand %}
-00000410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000420: 207b 2520 6966 206c 6973 7469 6e67 2e61   {% if listing.a
-00000430: 6374 696f 6e5f 6865 6164 6572 5f74 656d  ction_header_tem
-00000440: 706c 6174 655f 6e61 6d65 2025 7d0a 2020  plate_name %}.  
-00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000460: 2020 7b25 2069 6e63 6c75 6465 206c 6973    {% include lis
-00000470: 7469 6e67 2e61 6374 696f 6e5f 6865 6164  ting.action_head
-00000480: 6572 5f74 656d 706c 6174 655f 6e61 6d65  er_template_name
-00000490: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000004a0: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-000004b0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000004c0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-000004d0: 2020 2020 7b25 2062 6c6f 636b 206c 6973      {% block lis
-000004e0: 7469 6e67 2025 7d0a 2020 2020 2020 2020  ting %}.        
-000004f0: 2020 2020 2020 2020 3c74 6162 6c65 7b7b          <table{{
-00000500: 206c 6973 7469 6e67 2e61 7474 7273 207d   listing.attrs }
-00000510: 7d3e 0a20 2020 2020 2020 2020 2020 2020  }>.             
-00000520: 2020 2020 2020 207b 2520 626c 6f63 6b20         {% block 
-00000530: 6c69 7374 696e 675f 6865 6164 6572 2025  listing_header %
-00000540: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000550: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
-00000560: 6c69 7374 696e 672e 6861 735f 6865 6164  listing.has_head
-00000570: 6572 2025 7d0a 2020 2020 2020 2020 2020  er %}.          
-00000580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000590: 2020 3c74 6865 6164 3e0a 2020 2020 2020    <thead>.      
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 3c74 723e 0a20 2020 2020        <tr>.     
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
-000005e0: 7220 636f 6c20 696e 206c 6973 7469 6e67  r col in listing
-000005f0: 2e68 6561 6465 725f 636f 6c75 6d6e 7320  .header_columns 
-00000600: 257d 7b7b 2063 6f6c 2e68 746d 6c20 7d7d  %}{{ col.html }}
-00000610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000630: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
-00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000650: 2020 2020 2020 2020 2020 3c2f 7472 3e0a            </tr>.
-00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 2020 2020 2020 2020 2020 2020 3c2f 7468              </th
-00000680: 6561 643e 0a20 2020 2020 2020 2020 2020  ead>.           
-00000690: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000006a0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-000006b0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000006c0: 656e 6462 6c6f 636b 206c 6973 7469 6e67  endblock listing
-000006d0: 5f68 6561 6465 7220 257d 0a20 2020 2020  _header %}.     
-000006e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000006f0: 2520 626c 6f63 6b20 6c69 7374 696e 675f  % block listing_
-00000700: 626f 6479 2025 7d0a 2020 2020 2020 2020  body %}.        
+00000040: 6973 7469 6e67 2e63 7373 5f69 6420 7d7d  isting.css_id }}
+00000050: 220a 2020 2020 2020 2020 206c 6973 7469  ".         listi
+00000060: 6e67 2d73 7566 6669 783d 227b 7b20 6c69  ng-suffix="{{ li
+00000070: 7374 696e 672e 7375 6666 6978 207d 7d22  sting.suffix }}"
+00000080: 0a20 2020 2020 2020 2020 636c 6173 733d  .         class=
+00000090: 227b 7b20 6c69 7374 696e 675f 636f 6e74  "{{ listing_cont
+000000a0: 6169 6e65 725f 636c 6173 7320 7d7d 220a  ainer_class }}".
+000000b0: 2020 2020 2020 2020 2061 6a61 785f 7572           ajax_ur
+000000c0: 6c3d 227b 7b20 6c69 7374 696e 672e 6765  l="{{ listing.ge
+000000d0: 745f 7572 6c20 7d7d 220a 2020 2020 2020  t_url }}".      
+000000e0: 2020 207b 2520 6966 206c 6973 7469 6e67     {% if listing
+000000f0: 2e73 656c 6563 7469 6f6e 5f6d 656e 755f  .selection_menu_
+00000100: 6964 2025 7d73 656c 6563 7469 6f6e 2d6d  id %}selection-m
+00000110: 656e 752d 6964 3d22 7b7b 206c 6973 7469  enu-id="{{ listi
+00000120: 6e67 2e73 656c 6563 7469 6f6e 5f6d 656e  ng.selection_men
+00000130: 755f 6964 207d 7d22 7b25 2065 6e64 6966  u_id }}"{% endif
+00000140: 2025 7d0a 2020 2020 3e0a 2020 2020 3c73   %}.    >.    <s
+00000150: 7479 6c65 3e0a 2020 2020 2020 2020 406d  tyle>.        @m
+00000160: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
+00000170: 207b 7b20 6c69 7374 696e 672e 7468 656d   {{ listing.them
+00000180: 655f 6c6f 6361 6c69 7a65 645f 736d 616c  e_localized_smal
+00000190: 6c5f 6465 7669 6365 5f73 7479 6c65 735f  l_device_styles_
+000001a0: 7769 6474 6820 7d7d 2920 7b0a 2020 2020  width }}) {.    
+000001b0: 2020 2020 2020 7b25 2066 6f72 2073 7479        {% for sty
+000001c0: 6c65 2069 6e20 6c69 7374 696e 672e 6765  le in listing.ge
+000001d0: 745f 6c6f 6361 6c69 7a65 645f 736d 616c  t_localized_smal
+000001e0: 6c5f 6465 7669 6365 5f73 7479 6c65 7320  l_device_styles 
+000001f0: 257d 7b7b 2073 7479 6c65 207d 7d0a 2020  %}{{ style }}.  
+00000200: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+00000210: 7220 257d 0a20 2020 2020 2020 207d 0a20  r %}.        }. 
+00000220: 2020 203c 2f73 7479 6c65 3e0a 2020 2020     </style>.    
+00000230: 3c64 6976 2063 6c61 7373 3d22 6c69 7374  <div class="list
+00000240: 696e 672d 7370 696e 6e65 7222 3e3c 7370  ing-spinner"><sp
+00000250: 616e 2063 6c61 7373 3d22 7b7b 206c 6973  an class="{{ lis
+00000260: 7469 6e67 2e74 6865 6d65 5f73 7069 6e6e  ting.theme_spinn
+00000270: 6572 5f69 636f 6e20 7d7d 223e 3c2f 7370  er_icon }}"></sp
+00000280: 616e 3e3c 2f64 6976 3e0a 0a20 2020 2020  an></div>..     
+00000290: 2020 207b 2520 6966 206c 6973 7469 6e67     {% if listing
+000002a0: 2e72 6f77 5f66 6f72 6d5f 6572 726f 7273  .row_form_errors
+000002b0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000002c0: 3c75 6c20 636c 6173 733d 226c 6973 7469  <ul class="listi
+000002d0: 6e67 2d72 6f77 2d66 6f72 6d2d 6572 726f  ng-row-form-erro
+000002e0: 7273 223e 0a20 2020 2020 2020 2020 2020  rs">.           
+000002f0: 2020 2020 207b 2520 666f 7220 6572 726f       {% for erro
+00000300: 7220 696e 206c 6973 7469 6e67 2e72 6f77  r in listing.row
+00000310: 5f66 6f72 6d5f 6572 726f 7273 2025 7d3c  _form_errors %}<
+00000320: 6c69 3e7b 7b65 7272 6f72 7c73 6166 657d  li>{{error|safe}
+00000330: 7d3c 2f6c 693e 0a20 2020 2020 2020 2020  }</li>.         
+00000340: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
+00000350: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000360: 3c2f 756c 3e0a 2020 2020 2020 2020 7b25  </ul>.        {%
+00000370: 2065 6e64 6966 2025 7d0a 0a20 2020 2020   endif %}..     
+00000380: 2020 207b 2520 6966 206c 6973 7469 6e67     {% if listing
+00000390: 2e70 6167 696e 6174 6f72 2e63 6f75 6e74  .paginator.count
+000003a0: 206f 7220 6e6f 7420 6c69 7374 696e 672e   or not listing.
+000003b0: 656d 7074 795f 6c69 7374 696e 675f 7465  empty_listing_te
+000003c0: 6d70 6c61 7465 5f6e 616d 6520 257d 0a20  mplate_name %}. 
+000003d0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+000003e0: 2068 6173 5f74 6f70 5f74 6f6f 6c62 6172   has_top_toolbar
+000003f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000400: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000410: 746f 702d 746f 6f6c 6261 7222 3e0a 2020  top-toolbar">.  
+00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000430: 2020 7b25 2069 6e63 6c75 6465 206c 6973    {% include lis
+00000440: 7469 6e67 2e74 6f6f 6c62 6172 2e74 656d  ting.toolbar.tem
+00000450: 706c 6174 655f 6e61 6d65 2025 7d0a 2020  plate_name %}.  
+00000460: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000470: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000480: 207b 2520 656e 6469 6620 257d 0a0a 2020   {% endif %}..  
+00000490: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+000004a0: 6c69 7374 696e 672e 6361 6e5f 6564 6974  listing.can_edit
+000004b0: 206f 7220 6c69 7374 696e 672e 6861 735f   or listing.has_
+000004c0: 7570 6c6f 6164 206f 7220 6c69 7374 696e  upload or listin
+000004d0: 672e 6564 6974 5f6f 6e5f 6465 6d61 6e64  g.edit_on_demand
+000004e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000004f0: 2020 2020 7b25 2069 6620 6c69 7374 696e      {% if listin
+00000500: 672e 6163 7469 6f6e 5f68 6561 6465 725f  g.action_header_
+00000510: 7465 6d70 6c61 7465 5f6e 616d 6520 257d  template_name %}
+00000520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000530: 2020 2020 207b 2520 696e 636c 7564 6520       {% include 
+00000540: 6c69 7374 696e 672e 6163 7469 6f6e 5f68  listing.action_h
+00000550: 6561 6465 725f 7465 6d70 6c61 7465 5f6e  eader_template_n
+00000560: 616d 6520 257d 0a20 2020 2020 2020 2020  ame %}.         
+00000570: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+00000580: 257d 0a20 2020 2020 2020 2020 2020 207b  %}.            {
+00000590: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+000005a0: 2020 2020 2020 207b 2520 626c 6f63 6b20         {% block 
+000005b0: 6c69 7374 696e 6720 257d 0a20 2020 2020  listing %}.     
+000005c0: 2020 2020 2020 2020 2020 203c 7461 626c             <tabl
+000005d0: 657b 7b20 6c69 7374 696e 672e 6174 7472  e{{ listing.attr
+000005e0: 7320 7d7d 3e0a 2020 2020 2020 2020 2020  s }}>.          
+000005f0: 2020 2020 2020 2020 2020 7b25 2062 6c6f            {% blo
+00000600: 636b 206c 6973 7469 6e67 5f68 6561 6465  ck listing_heade
+00000610: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
+00000620: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00000630: 6966 206c 6973 7469 6e67 2e68 6173 5f68  if listing.has_h
+00000640: 6561 6465 7220 257d 0a20 2020 2020 2020  eader %}.       
+00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 203c 7468 6561 643e 0a20 2020       <thead>.   
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 2020 2020 2020 203c 7472 2063 6c61           <tr cla
+00000690: 7373 3d22 7b7b 2074 6865 6d65 5f63 6f6e  ss="{{ theme_con
+000006a0: 6669 672e 7468 656d 655f 726f 775f 636c  fig.theme_row_cl
+000006b0: 6173 7320 7d7d 223e 0a20 2020 2020 2020  ass }}">.       
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
+000006e0: 636f 6c20 696e 206c 6973 7469 6e67 2e68  col in listing.h
+000006f0: 6561 6465 725f 636f 6c75 6d6e 7320 257d  eader_columns %}
+00000700: 7b7b 2063 6f6c 2e68 746d 6c20 7d7d 0a20  {{ col.html }}. 
 00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 3c74 626f 6479 3e0a 2020 2020 2020 2020  <tbody>.        
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 7b25 2066 6f72 2072 6f77 2069 6e20 6c69  {% for row in li
-00000750: 7374 696e 672e 726f 7773 2025 7d7b 2520  sting.rows %}{% 
-00000760: 626c 6f63 6b20 6c69 7374 696e 675f 626f  block listing_bo
-00000770: 6479 5f72 6f77 2025 7d0a 2020 2020 2020  dy_row %}.      
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 3c74 727b 7b20 726f 772e        <tr{{ row.
-000007a0: 6174 7472 7320 7d7d 3e7b 2520 6966 206c  attrs }}>{% if l
-000007b0: 6973 7469 6e67 2e68 6173 5f68 6964 6465  isting.has_hidde
-000007c0: 6e5f 7365 6c65 6374 696f 6e20 257d 3c69  n_selection %}<i
-000007d0: 6e70 7574 2063 6c61 7373 3d22 726f 772d  nput class="row-
-000007e0: 7365 6c65 6374 2220 7479 7065 3d22 6869  select" type="hi
-000007f0: 6464 656e 2220 7b25 2069 6620 726f 772e  dden" {% if row.
-00000800: 7365 6c65 6374 6564 2025 7d6e 616d 653d  selected %}name=
-00000810: 2273 656c 6563 7465 645f 726f 7773 7b7b  "selected_rows{{
-00000820: 206c 6973 7469 6e67 2e73 7566 6669 7820   listing.suffix 
-00000830: 7d7d 2220 7b25 2065 6e64 6966 2025 7d73  }}" {% endif %}s
-00000840: 656c 6563 742d 6e61 6d65 3d22 7365 6c65  elect-name="sele
-00000850: 6374 6564 5f72 6f77 737b 7b20 6c69 7374  cted_rows{{ list
-00000860: 696e 672e 7375 6666 6978 207d 7d22 2076  ing.suffix }}" v
-00000870: 616c 7565 3d22 7b7b 2072 6f77 2e73 656c  alue="{{ row.sel
-00000880: 6563 7469 6f6e 5f76 616c 7565 207d 7d22  ection_value }}"
-00000890: 3e7b 2520 656e 6469 6620 257d 0a20 2020  >{% endif %}.   
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000008c0: 666f 7220 636f 6c20 696e 2072 6f77 2e63  for col in row.c
-000008d0: 6f6c 756d 6e73 2025 7d7b 7b20 636f 6c2e  olumns %}{{ col.
-000008e0: 6874 6d6c 207d 7d0a 2020 2020 2020 2020  html }}.        
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
-00000910: 7220 257d 3c2f 7472 3e7b 2520 656e 6462  r %}</tr>{% endb
-00000920: 6c6f 636b 206c 6973 7469 6e67 5f62 6f64  lock listing_bod
-00000930: 795f 726f 7720 257d 0a20 2020 2020 2020  y_row %}.       
-00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 207b 2520 656d 7074 7920 257d 0a20 2020   {% empty %}.   
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 2020 2020 2020 207b 2520 6966 206c           {% if l
-00000980: 6973 7469 6e67 2e65 6d70 7479 5f74 6162  isting.empty_tab
-00000990: 6c65 5f6d 7367 2025 7d0a 2020 2020 2020  le_msg %}.      
+00000720: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000730: 2520 656e 6466 6f72 2025 7d0a 2020 2020  % endfor %}.    
+00000740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000750: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 2020 2020 2020 2020 2020 3c2f 7468 6561            </thea
+00000780: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
+00000790: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+000007a0: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
+000007b0: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+000007c0: 6462 6c6f 636b 206c 6973 7469 6e67 5f68  dblock listing_h
+000007d0: 6561 6465 7220 257d 0a20 2020 2020 2020  eader %}.       
+000007e0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000007f0: 626c 6f63 6b20 6c69 7374 696e 675f 626f  block listing_bo
+00000800: 6479 2025 7d0a 2020 2020 2020 2020 2020  dy %}.          
+00000810: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00000820: 626f 6479 3e0a 2020 2020 2020 2020 2020  body>.          
+00000830: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00000840: 2066 6f72 2072 6f77 2069 6e20 6c69 7374   for row in list
+00000850: 696e 672e 726f 7773 2025 7d7b 2520 626c  ing.rows %}{% bl
+00000860: 6f63 6b20 6c69 7374 696e 675f 626f 6479  ock listing_body
+00000870: 5f72 6f77 2025 7d0a 2020 2020 2020 2020  _row %}.        
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2020 2020 3c74 727b 7b20 726f 772e 6174      <tr{{ row.at
+000008a0: 7472 7320 7d7d 3e7b 2520 6966 206c 6973  trs }}>{% if lis
+000008b0: 7469 6e67 2e68 6173 5f68 6964 6465 6e5f  ting.has_hidden_
+000008c0: 7365 6c65 6374 696f 6e20 257d 3c69 6e70  selection %}<inp
+000008d0: 7574 2063 6c61 7373 3d22 726f 772d 7365  ut class="row-se
+000008e0: 6c65 6374 2220 7479 7065 3d22 6869 6464  lect" type="hidd
+000008f0: 656e 2220 7b25 2069 6620 726f 772e 7365  en" {% if row.se
+00000900: 6c65 6374 6564 2025 7d6e 616d 653d 2273  lected %}name="s
+00000910: 656c 6563 7465 645f 726f 7773 7b7b 206c  elected_rows{{ l
+00000920: 6973 7469 6e67 2e73 7566 6669 7820 7d7d  isting.suffix }}
+00000930: 2220 7b25 2065 6e64 6966 2025 7d73 656c  " {% endif %}sel
+00000940: 6563 742d 6e61 6d65 3d22 7365 6c65 6374  ect-name="select
+00000950: 6564 5f72 6f77 737b 7b20 6c69 7374 696e  ed_rows{{ listin
+00000960: 672e 7375 6666 6978 207d 7d22 2076 616c  g.suffix }}" val
+00000970: 7565 3d22 7b7b 2072 6f77 2e73 656c 6563  ue="{{ row.selec
+00000980: 7469 6f6e 5f76 616c 7565 207d 7d22 3e7b  tion_value }}">{
+00000990: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
 000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009b0: 2020 2020 2020 2020 2020 7b25 2062 6c6f            {% blo
-000009c0: 636b 206c 6973 7469 6e67 5f65 6d70 7479  ck listing_empty
-000009d0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a20: 2020 2020 203c 7464 2063 6f6c 7370 616e       <td colspan
-00000a30: 3d22 7b7b 206e 625f 636f 6c75 6d6e 7320  ="{{ nb_columns 
-00000a40: 7d7d 223e 0a20 2020 2020 2020 2020 2020  }}">.           
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2020 2020 2020 2020 2020 207b 2520 666f             {% fo
+000009c0: 7220 636f 6c20 696e 2072 6f77 2e63 6f6c  r col in row.col
+000009d0: 756d 6e73 2025 7d7b 7b20 636f 6c2e 6874  umns %}{{ col.ht
+000009e0: 6d6c 207d 7d0a 2020 2020 2020 2020 2020  ml }}.          
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2020 2020 2020 7b25 2065 6e64 666f 7220        {% endfor 
+00000a10: 257d 3c2f 7472 3e7b 2520 656e 6462 6c6f  %}</tr>{% endblo
+00000a20: 636b 206c 6973 7469 6e67 5f62 6f64 795f  ck listing_body_
+00000a30: 726f 7720 257d 0a20 2020 2020 2020 2020  row %}.         
+00000a40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000a50: 2520 656d 7074 7920 257d 0a20 2020 2020  % empty %}.     
 00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 203c 6469 7620 636c 6173 733d 2265 6d70   <div class="emp
-00000a80: 7479 2d6d 6573 7361 6765 223e 0a20 2020  ty-message">.   
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 2020 2020 2020 207b 2520 6966 206c 6973         {% if lis
+00000a80: 7469 6e67 2e65 6d70 7479 5f74 6162 6c65  ting.empty_table
+00000a90: 5f6d 7367 2025 7d0a 2020 2020 2020 2020  _msg %}.        
 00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
-00000ac0: 6c69 7374 696e 672e 656d 7074 795f 7461  listing.empty_ta
-00000ad0: 626c 655f 6d73 6720 7d7d 0a20 2020 2020  ble_msg }}.     
+00000ab0: 2020 2020 2020 2020 7b25 2062 6c6f 636b          {% block
+00000ac0: 206c 6973 7469 6e67 5f65 6d70 7479 2025   listing_empty %
+00000ad0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
 00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000af0: 2020 2020 2020 3c74 723e 0a20 2020 2020        <tr>.     
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 2020 3c2f 7464 3e0a 2020 2020        </td>.    
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2020 203c 7464 2063 6f6c 7370 616e 3d22     <td colspan="
+00000b30: 7b7b 206e 625f 636f 6c75 6d6e 7320 7d7d  {{ nb_columns }}
+00000b40: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
 00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 3c2f 7472 3e0a 2020 2020 2020 2020 2020  </tr>.          
-00000b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b80: 2020 2020 2020 7b25 2065 6e64 626c 6f63        {% endbloc
-00000b90: 6b20 6c69 7374 696e 675f 656d 7074 7920  k listing_empty 
-00000ba0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00000bc0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
+00000b60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000b70: 6469 7620 636c 6173 733d 2265 6d70 7479  div class="empty
+00000b80: 2d6d 6573 7361 6765 223e 0a20 2020 2020  -message">.     
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2020 2020 2020 2020 207b 7b20 6c69             {{ li
+00000bc0: 7374 696e 672e 656d 7074 795f 7461 626c  sting.empty_tabl
+00000bd0: 655f 6d73 6720 7d7d 0a20 2020 2020 2020  e_msg }}.       
+00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 2020 2020 2020 2020 3c2f 7462 6f64 793e          </tbody>
-00000c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c20: 2020 2020 207b 2520 656e 6462 6c6f 636b       {% endblock
-00000c30: 206c 6973 7469 6e67 5f62 6f64 7920 257d   listing_body %}
-00000c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c50: 2020 2020 207b 2520 626c 6f63 6b20 6c69       {% block li
-00000c60: 7374 696e 675f 666f 6f74 6572 2025 7d0a  sting_footer %}.
+00000c00: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c30: 2020 2020 3c2f 7464 3e0a 2020 2020 2020      </td>.      
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000c60: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
 00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2020 7b25 2069 6620 6c69          {% if li
-00000c90: 7374 696e 672e 6861 735f 666f 6f74 6572  sting.has_footer
-00000ca0: 206f 7220 6c69 7374 696e 672e 666f 6f74   or listing.foot
-00000cb0: 6572 5f74 656d 706c 6174 655f 6e61 6d65  er_template_name
-00000cc0: 206f 7220 6c69 7374 696e 672e 7061 6769   or listing.pagi
-00000cd0: 6e61 746f 722e 696e 5f66 6f6f 7465 7220  nator.in_footer 
-00000ce0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000d00: 7466 6f6f 743e 0a20 2020 2020 2020 2020  tfoot>.         
+00000c80: 2020 2020 7b25 2065 6e64 626c 6f63 6b20      {% endblock 
+00000c90: 6c69 7374 696e 675f 656d 7074 7920 257d  listing_empty %}
+00000ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cb0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+00000cc0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ce0: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 2020 2020 2020 3c2f 7462 6f64 793e 0a20        </tbody>. 
 00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 2020 2020 2020 2020 7b25 2069 6620 6c69          {% if li
-00000d50: 7374 696e 672e 7061 6769 6e61 746f 722e  sting.paginator.
-00000d60: 696e 5f66 6f6f 7465 7220 257d 0a20 2020  in_footer %}.   
+00000d20: 2020 207b 2520 656e 6462 6c6f 636b 206c     {% endblock l
+00000d30: 6973 7469 6e67 5f62 6f64 7920 257d 0a20  isting_body %}. 
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 2020 207b 2520 626c 6f63 6b20 6c69 7374     {% block list
+00000d60: 696e 675f 666f 6f74 6572 2025 7d0a 2020  ing_footer %}.  
 00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d90: 203c 7464 2063 6f6c 7370 616e 3d22 7b7b   <td colspan="{{
-00000da0: 206e 625f 636f 6c75 6d6e 7320 7d7d 223e   nb_columns }}">
-00000db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dd0: 2020 2020 2020 2020 207b 2520 696e 636c           {% incl
-00000de0: 7564 6520 6c69 7374 696e 672e 7061 6769  ude listing.pagi
-00000df0: 6e61 746f 722e 7465 6d70 6c61 7465 5f6e  nator.template_n
-00000e00: 616d 6520 257d 0a20 2020 2020 2020 2020  ame %}.         
+00000d80: 2020 2020 2020 7b25 2069 6620 6c69 7374        {% if list
+00000d90: 696e 672e 6861 735f 666f 6f74 6572 206f  ing.has_footer o
+00000da0: 7220 6c69 7374 696e 672e 666f 6f74 6572  r listing.footer
+00000db0: 5f74 656d 706c 6174 655f 6e61 6d65 206f  _template_name o
+00000dc0: 7220 6c69 7374 696e 672e 7061 6769 6e61  r listing.pagina
+00000dd0: 746f 722e 696e 5f66 6f6f 7465 7220 257d  tor.in_footer %}
+00000de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000df0: 2020 2020 2020 2020 2020 2020 203c 7466               <tf
+00000e00: 6f6f 743e 0a20 2020 2020 2020 2020 2020  oot>.           
 00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2020 2020 2020 203c 2f74 643e             </td>
-00000e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 207b 2520 656c 6966 206c 6973 7469 6e67   {% elif listing
-00000e60: 2e66 6f6f 7465 725f 7465 6d70 6c61 7465  .footer_template
-00000e70: 5f6e 616d 6520 257d 0a20 2020 2020 2020  _name %}.       
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2020 2020 2020 2020 2020 203c 7464               <td
-00000ea0: 2063 6f6c 7370 616e 3d22 7b7b 206e 625f   colspan="{{ nb_
-00000eb0: 636f 6c75 6d6e 7320 7d7d 223e 0a20 2020  columns }}">.   
+00000e20: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e40: 2020 2020 2020 7b25 2069 6620 6c69 7374        {% if list
+00000e50: 696e 672e 7061 6769 6e61 746f 722e 696e  ing.paginator.in
+00000e60: 5f66 6f6f 7465 7220 257d 0a20 2020 2020  _footer %}.     
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000e90: 7464 2063 6f6c 7370 616e 3d22 7b7b 206e  td colspan="{{ n
+00000ea0: 625f 636f 6c75 6d6e 7320 7d7d 223e 0a20  b_columns }}">. 
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ee0: 2020 2020 207b 2520 696e 636c 7564 6520       {% include 
-00000ef0: 6c69 7374 696e 672e 666f 6f74 6572 5f74  listing.footer_t
-00000f00: 656d 706c 6174 655f 6e61 6d65 2025 7d0a  emplate_name %}.
+00000ed0: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
+00000ee0: 6520 6c69 7374 696e 672e 7061 6769 6e61  e listing.pagina
+00000ef0: 746f 722e 7465 6d70 6c61 7465 5f6e 616d  tor.template_nam
+00000f00: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
 00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2020 2020 3c2f 7464 3e0a 2020 2020 2020      </td>.      
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 2020 2020 2020 2020 7b25 2065 6c73            {% els
-00000f60: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-00000f90: 636f 6c20 696e 206c 6973 7469 6e67 2e66  col in listing.f
-00000fa0: 6f6f 7465 725f 636f 6c75 6d6e 7320 257d  ooter_columns %}
-00000fb0: 7b7b 2063 6f6c 2e68 746d 6c20 7d7d 0a20  {{ col.html }}. 
+00000f20: 2020 2020 2020 2020 203c 2f74 643e 0a20           </td>. 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000f50: 2520 656c 6966 206c 6973 7469 6e67 2e66  % elif listing.f
+00000f60: 6f6f 7465 725f 7465 6d70 6c61 7465 5f6e  ooter_template_n
+00000f70: 616d 6520 257d 0a20 2020 2020 2020 2020  ame %}.         
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 2020 2020 2020 2020 2020 203c 7464 2063             <td c
+00000fa0: 6f6c 7370 616e 3d22 7b7b 206e 625f 636f  olspan="{{ nb_co
+00000fb0: 6c75 6d6e 7320 7d7d 223e 0a20 2020 2020  lumns }}">.     
 00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fe0: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000fe0: 2020 207b 2520 696e 636c 7564 6520 6c69     {% include li
+00000ff0: 7374 696e 672e 666f 6f74 6572 5f74 656d  sting.footer_tem
+00001000: 706c 6174 655f 6e61 6d65 2025 7d0a 2020  plate_name %}.  
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001030: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
+00001030: 2020 3c2f 7464 3e0a 2020 2020 2020 2020    </td>.        
 00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 2020 2020 2020 3c2f 7466 6f6f            </tfoo
-00001060: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
-00001070: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00001080: 6469 6620 257d 0a20 2020 2020 2020 2020  dif %}.         
-00001090: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-000010a0: 6462 6c6f 636b 206c 6973 7469 6e67 5f66  dblock listing_f
-000010b0: 6f6f 7465 7220 257d 0a20 2020 2020 2020  ooter %}.       
-000010c0: 2020 2020 2020 2020 203c 2f74 6162 6c65           </table
-000010d0: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-000010e0: 2065 6e64 626c 6f63 6b20 6c69 7374 696e   endblock listin
-000010f0: 6720 257d 0a0a 2020 2020 2020 2020 2020  g %}..          
-00001100: 2020 7b25 2062 6c6f 636b 2068 6964 6465    {% block hidde
-00001110: 6e73 2025 7d0a 2020 2020 2020 2020 2020  ns %}.          
-00001120: 2020 2020 2020 7b25 2066 6f72 2068 6964        {% for hid
-00001130: 6465 6e20 696e 206c 6973 7469 6e67 2e66  den in listing.f
-00001140: 6f72 6d5f 696e 7075 745f 6869 6464 656e  orm_input_hidden
-00001150: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
-00001160: 2020 2020 2020 2020 203c 696e 7075 7420           <input 
-00001170: 7479 7065 3d22 6869 6464 656e 2220 6e61  type="hidden" na
-00001180: 6d65 3d22 7b7b 2068 6964 6465 6e2e 3020  me="{{ hidden.0 
-00001190: 7d7d 2220 7661 6c75 653d 227b 7b20 6869  }}" value="{{ hi
-000011a0: 6464 656e 2e31 207d 7d22 3e7b 2520 656e  dden.1 }}">{% en
-000011b0: 6466 6f72 2025 7d0a 2020 2020 2020 2020  dfor %}.        
-000011c0: 2020 2020 2020 2020 7b25 2069 6620 6c69          {% if li
-000011d0: 7374 696e 672e 6564 6974 6162 6c65 2061  sting.editable a
-000011e0: 6e64 206c 6973 7469 6e67 2e65 6469 7469  nd listing.editi
-000011f0: 6e67 2025 7d0a 2020 2020 2020 2020 2020  ng %}.          
-00001200: 2020 2020 2020 2020 2020 7b25 2066 6f72            {% for
-00001210: 2068 6964 6465 6e5f 6669 656c 6420 696e   hidden_field in
-00001220: 206c 6973 7469 6e67 2e65 6469 7469 6e67   listing.editing
-00001230: 5f68 6964 6465 6e5f 666f 726d 5f66 6965  _hidden_form_fie
-00001240: 6c64 7320 257d 0a20 2020 2020 2020 2020  lds %}.         
-00001250: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00001260: 7b20 6869 6464 656e 5f66 6965 6c64 207d  { hidden_field }
-00001270: 7d7b 2520 656e 6466 6f72 2025 7d0a 2020  }{% endfor %}.  
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 7b7b 206c 6973 7469 6e67 2e67 6574    {{ listing.get
-000012a0: 5f66 6f72 6d73 6574 2e6d 616e 6167 656d  _formset.managem
-000012b0: 656e 745f 666f 726d 207d 7d0a 2020 2020  ent_form }}.    
-000012c0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000012d0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-000012e0: 2020 2020 7b25 2065 6e64 626c 6f63 6b20      {% endblock 
-000012f0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
-00001300: 7b25 2069 6620 6c69 7374 696e 672e 6361  {% if listing.ca
-00001310: 6e5f 6564 6974 206f 7220 6c69 7374 696e  n_edit or listin
-00001320: 672e 6861 735f 7570 6c6f 6164 206f 7220  g.has_upload or 
-00001330: 6c69 7374 696e 672e 6564 6974 5f6f 6e5f  listing.edit_on_
-00001340: 6465 6d61 6e64 2025 7d0a 2020 2020 2020  demand %}.      
-00001350: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
-00001360: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-00001370: 2065 6e64 6966 2025 7d0a 0a20 2020 2020   endif %}..     
-00001380: 2020 2020 2020 207b 2520 6966 2068 6173         {% if has
-00001390: 5f62 6f74 746f 6d5f 746f 6f6c 6261 7220  _bottom_toolbar 
-000013a0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-000013b0: 2020 203c 6469 7620 636c 6173 733d 2262     <div class="b
-000013c0: 6f74 746f 6d2d 746f 6f6c 6261 7222 3e0a  ottom-toolbar">.
-000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013e0: 2020 2020 7b25 2069 6e63 6c75 6465 206c      {% include l
-000013f0: 6973 7469 6e67 2e74 6f6f 6c62 6172 2e74  isting.toolbar.t
-00001400: 656d 706c 6174 655f 6e61 6d65 2025 7d0a  emplate_name %}.
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00001430: 2020 207b 2520 656e 6469 6620 257d 0a0a     {% endif %}..
-00001440: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00001450: 6620 6c69 7374 696e 672e 6861 735f 7061  f listing.has_pa
-00001460: 6769 6e61 746f 7220 616e 6420 6e6f 7420  ginator and not 
-00001470: 6c69 7374 696e 672e 7061 6769 6e61 746f  listing.paginato
-00001480: 722e 696e 5f66 6f6f 7465 7220 257d 0a20  r.in_footer %}. 
-00001490: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000014a0: 2520 696e 636c 7564 6520 6c69 7374 696e  % include listin
-000014b0: 672e 7061 6769 6e61 746f 722e 7465 6d70  g.paginator.temp
-000014c0: 6c61 7465 5f6e 616d 6520 257d 0a20 2020  late_name %}.   
-000014d0: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
-000014e0: 6620 257d 0a0a 2020 2020 2020 2020 2020  f %}..          
-000014f0: 2020 7b25 2069 6620 6c69 7374 696e 672e    {% if listing.
-00001500: 6361 6e5f 6564 6974 206f 7220 6c69 7374  can_edit or list
-00001510: 696e 672e 6861 735f 7570 6c6f 6164 206f  ing.has_upload o
-00001520: 7220 6c69 7374 696e 672e 6564 6974 5f6f  r listing.edit_o
-00001530: 6e5f 6465 6d61 6e64 2025 7d0a 2020 2020  n_demand %}.    
-00001540: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00001550: 6620 6c69 7374 696e 672e 6163 7469 6f6e  f listing.action
-00001560: 5f66 6f6f 7465 725f 7465 6d70 6c61 7465  _footer_template
-00001570: 5f6e 616d 6520 257d 0a20 2020 2020 2020  _name %}.       
-00001580: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00001590: 696e 636c 7564 6520 6c69 7374 696e 672e  include listing.
-000015a0: 6163 7469 6f6e 5f66 6f6f 7465 725f 7465  action_footer_te
-000015b0: 6d70 6c61 7465 5f6e 616d 6520 257d 0a20  mplate_name %}. 
-000015c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000015d0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-000015e0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-000015f0: 257d 0a20 2020 2020 2020 207b 2520 656c  %}.        {% el
-00001600: 7365 2025 7d0a 2020 2020 2020 2020 2020  se %}.          
-00001610: 2020 7b25 2069 6620 6c69 7374 696e 672e    {% if listing.
-00001620: 6361 6e5f 6564 6974 206f 7220 6c69 7374  can_edit or list
-00001630: 696e 672e 6861 735f 7570 6c6f 6164 206f  ing.has_upload o
-00001640: 7220 6c69 7374 696e 672e 6564 6974 5f6f  r listing.edit_o
-00001650: 6e5f 6465 6d61 6e64 2025 7d0a 2020 2020  n_demand %}.    
-00001660: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
-00001670: 6620 6c69 7374 696e 672e 6163 7469 6f6e  f listing.action
-00001680: 5f68 6561 6465 725f 7465 6d70 6c61 7465  _header_template
-00001690: 5f6e 616d 6520 257d 0a20 2020 2020 2020  _name %}.       
-000016a0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-000016b0: 696e 636c 7564 6520 6c69 7374 696e 672e  include listing.
-000016c0: 6163 7469 6f6e 5f68 6561 6465 725f 7465  action_header_te
-000016d0: 6d70 6c61 7465 5f6e 616d 6520 257d 0a20  mplate_name %}. 
-000016e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000016f0: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00001700: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00001710: 257d 0a20 2020 2020 2020 2020 2020 207b  %}.            {
-00001720: 2520 696e 636c 7564 6520 6c69 7374 696e  % include listin
-00001730: 672e 656d 7074 795f 6c69 7374 696e 675f  g.empty_listing_
-00001740: 7465 6d70 6c61 7465 5f6e 616d 6520 257d  template_name %}
-00001750: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00001760: 6966 206c 6973 7469 6e67 2e63 616e 5f65  if listing.can_e
-00001770: 6469 7420 6f72 206c 6973 7469 6e67 2e68  dit or listing.h
-00001780: 6173 5f75 706c 6f61 6420 6f72 206c 6973  as_upload or lis
-00001790: 7469 6e67 2e65 6469 745f 6f6e 5f64 656d  ting.edit_on_dem
-000017a0: 616e 6420 257d 0a20 2020 2020 2020 2020  and %}.         
-000017b0: 2020 2020 2020 207b 2520 6966 206c 6973         {% if lis
-000017c0: 7469 6e67 2e61 6374 696f 6e5f 666f 6f74  ting.action_foot
-000017d0: 6572 5f74 656d 706c 6174 655f 6e61 6d65  er_template_name
-000017e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000017f0: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
-00001800: 6465 206c 6973 7469 6e67 2e61 6374 696f  de listing.actio
-00001810: 6e5f 666f 6f74 6572 5f74 656d 706c 6174  n_footer_templat
-00001820: 655f 6e61 6d65 2025 7d0a 2020 2020 2020  e_name %}.      
-00001830: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-00001840: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
-00001850: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
-00001860: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
-00001870: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
-00001880: 6966 2025 7d0a 0a20 2020 203c 2f64 6976  if %}..    </div
-00001890: 3e0a 7b25 2065 6e64 6175 746f 6573 6361  >.{% endautoesca
-000018a0: 7065 2025 7d                             pe %}
+00001050: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+00001060: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 2020 207b 2520 666f 7220 636f         {% for co
+00001090: 6c20 696e 206c 6973 7469 6e67 2e66 6f6f  l in listing.foo
+000010a0: 7465 725f 636f 6c75 6d6e 7320 257d 7b7b  ter_columns %}{{
+000010b0: 2063 6f6c 2e68 746d 6c20 7d7d 0a20 2020   col.html }}.   
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+00001110: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 2020 3c2f 7466 6f6f 743e          </tfoot>
+00001160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001170: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00001180: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00001190: 2020 2020 2020 2020 207b 2520 656e 6462           {% endb
+000011a0: 6c6f 636b 206c 6973 7469 6e67 5f66 6f6f  lock listing_foo
+000011b0: 7465 7220 257d 0a20 2020 2020 2020 2020  ter %}.         
+000011c0: 2020 2020 2020 203c 2f74 6162 6c65 3e0a         </table>.
+000011d0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000011e0: 6e64 626c 6f63 6b20 6c69 7374 696e 6720  ndblock listing 
+000011f0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+00001200: 7b25 2062 6c6f 636b 2068 6964 6465 6e73  {% block hiddens
+00001210: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001220: 2020 2020 7b25 2066 6f72 2068 6964 6465      {% for hidde
+00001230: 6e20 696e 206c 6973 7469 6e67 2e66 6f72  n in listing.for
+00001240: 6d5f 696e 7075 745f 6869 6464 656e 7320  m_input_hiddens 
+00001250: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
+00001260: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
+00001270: 7065 3d22 6869 6464 656e 2220 6e61 6d65  pe="hidden" name
+00001280: 3d22 7b7b 2068 6964 6465 6e2e 3020 7d7d  ="{{ hidden.0 }}
+00001290: 2220 7661 6c75 653d 227b 7b20 6869 6464  " value="{{ hidd
+000012a0: 656e 2e31 207d 7d22 3e7b 2520 656e 6466  en.1 }}">{% endf
+000012b0: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
+000012c0: 2020 2020 2020 7b25 2069 6620 6c69 7374        {% if list
+000012d0: 696e 672e 6564 6974 6162 6c65 2061 6e64  ing.editable and
+000012e0: 206c 6973 7469 6e67 2e65 6469 7469 6e67   listing.editing
+000012f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001300: 2020 2020 2020 2020 7b25 2066 6f72 2068          {% for h
+00001310: 6964 6465 6e5f 6669 656c 6420 696e 206c  idden_field in l
+00001320: 6973 7469 6e67 2e65 6469 7469 6e67 5f68  isting.editing_h
+00001330: 6964 6465 6e5f 666f 726d 5f66 6965 6c64  idden_form_field
+00001340: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
+00001350: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00001360: 6869 6464 656e 5f66 6965 6c64 207d 7d7b  hidden_field }}{
+00001370: 2520 656e 6466 6f72 2025 7d0a 2020 2020  % endfor %}.    
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 7b7b 206c 6973 7469 6e67 2e67 6574 5f66  {{ listing.get_f
+000013a0: 6f72 6d73 6574 2e6d 616e 6167 656d 656e  ormset.managemen
+000013b0: 745f 666f 726d 207d 7d0a 2020 2020 2020  t_form }}.      
+000013c0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+000013d0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+000013e0: 2020 7b25 2065 6e64 626c 6f63 6b20 257d    {% endblock %}
+000013f0: 0a0a 2020 2020 2020 2020 2020 2020 7b25  ..            {%
+00001400: 2069 6620 6c69 7374 696e 672e 6361 6e5f   if listing.can_
+00001410: 6564 6974 206f 7220 6c69 7374 696e 672e  edit or listing.
+00001420: 6861 735f 7570 6c6f 6164 206f 7220 6c69  has_upload or li
+00001430: 7374 696e 672e 6564 6974 5f6f 6e5f 6465  sting.edit_on_de
+00001440: 6d61 6e64 2025 7d0a 2020 2020 2020 2020  mand %}.        
+00001450: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
+00001460: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00001470: 6e64 6966 2025 7d0a 0a20 2020 2020 2020  ndif %}..       
+00001480: 2020 2020 207b 2520 6966 2068 6173 5f62       {% if has_b
+00001490: 6f74 746f 6d5f 746f 6f6c 6261 7220 257d  ottom_toolbar %}
+000014a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000014b0: 203c 6469 7620 636c 6173 733d 2262 6f74   <div class="bot
+000014c0: 746f 6d2d 746f 6f6c 6261 7222 3e0a 2020  tom-toolbar">.  
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 7b25 2069 6e63 6c75 6465 206c 6973    {% include lis
+000014f0: 7469 6e67 2e74 6f6f 6c62 6172 2e74 656d  ting.toolbar.tem
+00001500: 706c 6174 655f 6e61 6d65 2025 7d0a 2020  plate_name %}.  
+00001510: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001520: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00001530: 207b 2520 656e 6469 6620 257d 0a0a 2020   {% endif %}..  
+00001540: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001550: 6c69 7374 696e 672e 6861 735f 7061 6769  listing.has_pagi
+00001560: 6e61 746f 7220 616e 6420 6e6f 7420 6c69  nator and not li
+00001570: 7374 696e 672e 7061 6769 6e61 746f 722e  sting.paginator.
+00001580: 696e 5f66 6f6f 7465 7220 257d 0a20 2020  in_footer %}.   
+00001590: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000015a0: 696e 636c 7564 6520 6c69 7374 696e 672e  include listing.
+000015b0: 7061 6769 6e61 746f 722e 7465 6d70 6c61  paginator.templa
+000015c0: 7465 5f6e 616d 6520 257d 0a20 2020 2020  te_name %}.     
+000015d0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000015e0: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+000015f0: 7b25 2069 6620 6c69 7374 696e 672e 6361  {% if listing.ca
+00001600: 6e5f 6564 6974 206f 7220 6c69 7374 696e  n_edit or listin
+00001610: 672e 6861 735f 7570 6c6f 6164 206f 7220  g.has_upload or 
+00001620: 6c69 7374 696e 672e 6564 6974 5f6f 6e5f  listing.edit_on_
+00001630: 6465 6d61 6e64 2025 7d0a 2020 2020 2020  demand %}.      
+00001640: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001650: 6c69 7374 696e 672e 6163 7469 6f6e 5f66  listing.action_f
+00001660: 6f6f 7465 725f 7465 6d70 6c61 7465 5f6e  ooter_template_n
+00001670: 616d 6520 257d 0a20 2020 2020 2020 2020  ame %}.         
+00001680: 2020 2020 2020 2020 2020 207b 2520 696e             {% in
+00001690: 636c 7564 6520 6c69 7374 696e 672e 6163  clude listing.ac
+000016a0: 7469 6f6e 5f66 6f6f 7465 725f 7465 6d70  tion_footer_temp
+000016b0: 6c61 7465 5f6e 616d 6520 257d 0a20 2020  late_name %}.   
+000016c0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000016d0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+000016e0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000016f0: 0a20 2020 2020 2020 207b 2520 656c 7365  .        {% else
+00001700: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001710: 7b25 2069 6620 6c69 7374 696e 672e 6361  {% if listing.ca
+00001720: 6e5f 6564 6974 206f 7220 6c69 7374 696e  n_edit or listin
+00001730: 672e 6861 735f 7570 6c6f 6164 206f 7220  g.has_upload or 
+00001740: 6c69 7374 696e 672e 6564 6974 5f6f 6e5f  listing.edit_on_
+00001750: 6465 6d61 6e64 2025 7d0a 2020 2020 2020  demand %}.      
+00001760: 2020 2020 2020 2020 2020 7b25 2069 6620            {% if 
+00001770: 6c69 7374 696e 672e 6163 7469 6f6e 5f68  listing.action_h
+00001780: 6561 6465 725f 7465 6d70 6c61 7465 5f6e  eader_template_n
+00001790: 616d 6520 257d 0a20 2020 2020 2020 2020  ame %}.         
+000017a0: 2020 2020 2020 2020 2020 207b 2520 696e             {% in
+000017b0: 636c 7564 6520 6c69 7374 696e 672e 6163  clude listing.ac
+000017c0: 7469 6f6e 5f68 6561 6465 725f 7465 6d70  tion_header_temp
+000017d0: 6c61 7465 5f6e 616d 6520 257d 0a20 2020  late_name %}.   
+000017e0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
+000017f0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00001800: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00001810: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00001820: 696e 636c 7564 6520 6c69 7374 696e 672e  include listing.
+00001830: 656d 7074 795f 6c69 7374 696e 675f 7465  empty_listing_te
+00001840: 6d70 6c61 7465 5f6e 616d 6520 257d 0a20  mplate_name %}. 
+00001850: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00001860: 206c 6973 7469 6e67 2e63 616e 5f65 6469   listing.can_edi
+00001870: 7420 6f72 206c 6973 7469 6e67 2e68 6173  t or listing.has
+00001880: 5f75 706c 6f61 6420 6f72 206c 6973 7469  _upload or listi
+00001890: 6e67 2e65 6469 745f 6f6e 5f64 656d 616e  ng.edit_on_deman
+000018a0: 6420 257d 0a20 2020 2020 2020 2020 2020  d %}.           
+000018b0: 2020 2020 207b 2520 6966 206c 6973 7469       {% if listi
+000018c0: 6e67 2e61 6374 696f 6e5f 666f 6f74 6572  ng.action_footer
+000018d0: 5f74 656d 706c 6174 655f 6e61 6d65 2025  _template_name %
+000018e0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000018f0: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00001900: 206c 6973 7469 6e67 2e61 6374 696f 6e5f   listing.action_
+00001910: 666f 6f74 6572 5f74 656d 706c 6174 655f  footer_template_
+00001920: 6e61 6d65 2025 7d0a 2020 2020 2020 2020  name %}.        
+00001930: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+00001940: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00001950: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00001960: 2020 2020 2020 2020 7b25 2069 6620 6c69          {% if li
+00001970: 7374 696e 672e 6361 6e5f 6564 6974 206f  sting.can_edit o
+00001980: 7220 6c69 7374 696e 672e 6861 735f 7570  r listing.has_up
+00001990: 6c6f 6164 206f 7220 6c69 7374 696e 672e  load or listing.
+000019a0: 6564 6974 5f6f 6e5f 6465 6d61 6e64 2025  edit_on_demand %
+000019b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000019c0: 2020 3c2f 666f 726d 3e0a 2020 2020 2020    </form>.      
+000019d0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+000019e0: 7d0a 2020 2020 2020 2020 7b25 2065 6e64  }.        {% end
+000019f0: 6966 2025 7d0a 0a20 2020 203c 2f64 6976  if %}..    </div
+00001a00: 3e0a 7b25 2065 6e64 6175 746f 6573 6361  >.{% endautoesca
+00001a10: 7065 2025 7d                             pe %}
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/footer.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/footer.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,71 @@
 {% load static %}
 {% load django_listing %}
 <div id="listing-popup-container"></div>
 <script type="text/javascript">
     var csrf_token = '{{ csrf_token }}';
     $(document).ready(function () {
         $.ajaxSetup({
-            data: { 'csrfmiddlewaretoken':csrf_token  }
+            data: {'csrfmiddlewaretoken': csrf_token}
         });
     });
 </script>
-<script src="{% static 'django_listing/js/django_listing.js' %}"></script>
-
+{% if AUTO_DECLARE_JS %}
+    <script src="{% static 'django_listing/js/django_listing.min.js' %}?{{ STATIC_FILES_VERSION }}"></script>
+{% endif %}
 {% if need_media_for.datetimepicker and DATETIMEPICKER_JS_URL %}
     {% block django_listing_datepicker %}
-    <script src="{{ DATETIMEPICKER_JS_URL }}"></script>
-    {% get_dict_list "datetimepickers" as dict_list %}
-    <script type="text/javascript">
-        $(document).ready(function () {
-            {% for dct in dict_list %}
-                $('#{{dct.div_id}} .edit-datecolumn').datetimepicker({timepicker:false, format:'{{dct.listing.datetimepicker_date_format}}'});
-                $('#{{dct.div_id}} .edit-datetimecolumn').datetimepicker({format:'{{dct.listing.datetimepicker_datetime_format}}'});
-                $('#{{dct.div_id}} .edit-timecolumn').datetimepicker({datepicker:false, format:'{{dct.listing.datetimepicker_time_format}}'});
-            {% endfor %}
-        });
-    </script>
+        {% if AUTO_DECLARE_JS %}
+            <script src="{{ DATETIMEPICKER_JS_URL }}?{{ STATIC_FILES_VERSION }}"></script>
+        {% endif %}
+        {% get_dict_list "datetimepickers" as dict_list %}
+        <script type="text/javascript">
+            $(document).ready(function () {
+                {% for dct in dict_list %}
+                    $('#{{dct.div_id}} .edit-datecolumn').datetimepicker({
+                        timepicker: false,
+                        format: '{{dct.listing.datetimepicker_date_format}}'
+                    });
+                    $('#{{dct.div_id}} .edit-datetimecolumn').datetimepicker({format: '{{dct.listing.datetimepicker_datetime_format}}'});
+                    $('#{{dct.div_id}} .edit-timecolumn').datetimepicker({
+                        datepicker: false,
+                        format: '{{dct.listing.datetimepicker_time_format}}'
+                    });
+                {% endfor %}
+            });
+        </script>
     {% endblock %}
 {% endif %}
 
 {% if need_media_for.dropzone and DROPZONE_JS_URL %}
-    <script src="{{ DROPZONE_JS_URL }}"></script>
+    {% if AUTO_DECLARE_JS %}
+        <script src="{{ DROPZONE_JS_URL }}?{{ STATIC_FILES_VERSION }}"></script>
+    {% endif %}
     {% get_dict_list "dropzones" as dict_list %}
     <script type="text/javascript">
-        var listing_div_id = '{{ listing.id|underscore_to_dash }}';
+        var listing_div_id = '{{ listing.css_id }}';
         {% for dct in dict_list %}
-        Dropzone.options.{{ dct.dz_camel_name}} = {{ dct.options|json_options }};
+            Dropzone.options.{{ dct.dz_camel_name}} = {{ dct.options|json_options }};
         {% endfor %}
     </script>
 
 {% endif %}
 
+{% if need_media_for.autocomplete and AUTOCOMPLETE_JS_URLS %}
+    {% block django_listing_autocomplete %}
+        {% if AUTO_DECLARE_JS %}
+            {% for url in AUTOCOMPLETE_JS_URLS %}
+                <script src="{{ url }}?{{ STATIC_FILES_VERSION }}"></script>
+            {% endfor %}
+        {% endif %}
+    {% endblock %}
+{% endif %}
+
 {% footer_snippets %}
 
 {% if request.django_listing_onready_snippets %}
     <script type="text/javascript">
-    $(document).ready(function () {
-        {% onready_snippets %}
-    });
+        $(document).ready(function () {
+            {% onready_snippets %}
+        });
     </script>
 {% endif %}
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/view_object_popup.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/view_object_popup.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <div class="modal fade" id="listing-popup" tabindex="-1" role="dialog" aria-hidden="true">
     <div class="modal-dialog modal-dialog-centered" role="document">
         <div class="modal-content">
             <div class="modal-header">
                 <h5 class="modal-title">{{ object }}</h5>
-                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
-                    <span aria-hidden="true">&times;</span>
-                </button>
+                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
             </div>
             <div class="modal-body">
 
                 <table class="object-popup">
                     {% for row in rows %}
                         <tr>
                             {% for label, value in row %}
@@ -21,12 +19,12 @@
                             {% endfor %}
                         </tr>
                     {% endfor %}
                 </table>
 
             </div>
             <div class="modal-footer">
-                <button type="button" class="btn btn-primary" data-dismiss="modal">Close</button>
+                <button type="button" class="btn btn-primary" data-bs-dismiss="modal">Close</button>
             </div>
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,4 +1,3 @@
 ** {{ object }} **
- ×
 {{ value|safe }} {{ label }}{{ label_ending }}
 Close
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/filters_form.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/filters_form.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/listing_div.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/listing_div.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "django_listing/listing.html" %}
+{% extends "./listing.html" %}
 {% block listing %}
     <div{{ listing.attrs }}>
         {% for row in listing.div_rows %}
             <div{{ row.attrs }}>
             {% if listing.can_select %}
                 <input class="row-select" type="hidden" select-name="selected_rows{{ listing.suffix }}" value="{{ row.selection_value }}">
                 {% if listing.selection_has_overlay %}
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/tbi_select.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/tbi_select.html`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/action_header.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/action_header.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load django_listing %}
 <form method="post"
       {% comment %}Be careful, for dropzone, action="..." must be NOT empty : use at lease "#"{% endcomment %}
       action="{% if listing.anchor_hash is not None %}#{{ listing.anchor_hash }}{% else %}{% if listing.has_upload %}#{% endif %}{% endif %}"
       enctype="multipart/form-data"
-      id="action-form{{ listing.suffix|underscore_to_dash }}"
+      id="action-form{{ listing.css_suffix }}"
       class="action-form{% if listing.has_upload %} dropzone{% endif %}">
 {% if listing.has_upload %}
     <div class="drag-overlay"><div class="overlay-inner"><span class="listing-icon-upload-cloud"></span></div></div>
 {% endif %}
 <input type="hidden" name="csrfmiddlewaretoken" value="{{ csrf_token }}">
 <input type="hidden" name="action" value="" class="action-hidden-value">
 <div class="dz-message" style="margin: 0"></div>
```

### Comparing `django-listing-0.0.9/django_listing/templates/django_listing/actions_buttons.html` & `django-listing-0.5.0/django_listing/templates/django_listing/default/actions_buttons.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% load django_listing %}
 {% block actions_buttons %}{% spaceless %}
 <form method="post">
 <input type="hidden" name="csrfmiddlewaretoken" value="{{ csrf_token }}">
-<input type="hidden" name="listing_id" value="{{ listing.id|underscore_to_dash }}">
+<input type="hidden" name="listing_id" value="{{ listing.css_id }}">
 <input type="hidden" name="action" value="action_button">
 <input type="hidden" name="action_pk" value="{{ rec.pk }}">
 <input type="hidden" name="action_col" value="{{ action_col }}">
     <ul class="actions-buttons">
         {% for button in buttons %}
             <li class="{{ button.theme_li_class }} {{ button.name_css_class }}{% if button.disabled %} disabled{% endif %}">
-                {% if button.type == "link" %}
-                    <a class="listing-nav {{ button.theme_button_class }}{% if button.disabled %} disabled{% endif %}" role="button"{% if not button.disabled %} href="{{ button.url }}"{% endif %}{% if button.title %} title="{{ button.title }}"{% endif %}>{% if button.icon and button.has_icon %}<span class="{{ button.icon }} icon"></span> {% endif %}{% if button.text and button.has_text %}<span class="text">{{ button.text }}</span>{% endif %}</a>
+                {% if button.type == "link" or button.type == "extlink" %}
+                    <a class="{% if button.type == "link" %}listing-nav {% endif %}{{ button.theme_button_class }}{% if button.disabled %} disabled{% endif %}" role="button"{% if not button.disabled %} href="{{ button.url }}"{% endif %}{% if button.title %} title="{{ button.title }}"{% endif %}>{% if button.icon and button.has_icon %}<span class="{{ button.icon }} icon"></span> {% endif %}{% if button.text and button.has_text %}<span class="text">{{ button.text }}</span>{% endif %}</a>
                 {% else %}
                     <button type="{{ button.type }}" name="action_button" value="{{ button.name }}"{% if button.title %} title="{{ button.title }}"{% endif %} class="listing-nav {{ button.theme_button_class }}{% if button.disabled %} disabled{% endif %}" role="button">{% if button.icon and button.has_icon %}<span class="{{ button.icon }} icon"></span> {% endif %}{% if button.text and button.has_text%}<span class="text">{{ button.text }}</span>{% endif %}</button>
                 {% endif %}
             </li>
         {% endfor %}
     </ul>
 </form>
```

### Comparing `django-listing-0.0.9/django_listing/context.py` & `django-listing-0.5.0/django_listing/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #
 # Created : 2018-02-10
 #
 # @author: Eric Lapouyade
 #
 
 import pprint
+
 pp = pprint.PrettyPrinter(indent=4)
 import types
 
-__all__ = ['RenderContext']
+__all__ = ["RenderContext"]
+
 
 def isgenerator(arg):
     return isinstance(arg, types.GeneratorType)
 
+
 # Simplistic context object : just a dict accessible with attribute notation
 class RenderContext(dict):
     def __init__(self, *args, **kwargs):
         """
         If we're initialized with a dict, make sure we turn all the
         subdicts into Dicts as well.
         """
@@ -29,15 +32,15 @@
             elif isinstance(arg, tuple) and (not isinstance(arg[0], tuple)):
                 self[arg[0]] = arg[1]
             elif isinstance(arg, (list, tuple)) or isgenerator(arg):
                 for key, val in arg:
                     self[key] = val
             # other types of postionnal arguments are not injected into the context
 
-
         for key, val in kwargs.items():
             self[key] = val
 
     def __getattr__(self, attr):
         return self[attr]
+
     def __setattr__(self, attr, value):
-        self[attr] = value
+        self[attr] = value
```

### Comparing `django-listing-0.0.9/django_listing/utils.py` & `django-listing-0.5.0/django_listing/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 #
 # Created : 2018-04-01
 #
 # @author: Eric Lapouyade
 #
 import copy
 import pprint
+
 pp = pprint.PrettyPrinter(indent=4)
 
 
-def normalize_list(value, separator=',', transform=str.strip, default='',force_length=None):
+def normalize_list(
+    value, separator=",", transform=str.strip, default="", force_length=None
+):
     if isinstance(value, str):
         value = list(map(transform, value.split(separator)))
     if force_length:
         length = len(value)
         if force_length < length:
             value = value[:force_length]
         elif force_length > length:
             value = value + [default] * (force_length - length)
     return value
 
 
 def normalize_choices(choices, int_keys=False):
     normalized_choices = []
-    if isinstance(choices,str):
-        for c in choices.split(','):
-            if ':' in c:
-                normalized_choices.append(c.split(':',1))
+    if isinstance(choices, str):
+        for c in choices.split(","):
+            if ":" in c:
+                normalized_choices.append(c.split(":", 1))
             else:
-                normalized_choices.append([c,c])
-    elif isinstance(choices, (tuple,list)):
+                normalized_choices.append([c, c])
+    elif isinstance(choices, (tuple, list)):
         for c in choices:
             if isinstance(c, str):
-                normalized_choices.append([c,c])
-            elif isinstance(c,(tuple,list)):
+                normalized_choices.append([c, c])
+            elif isinstance(c, (tuple, list)):
                 if len(c) == 1:
-                    normalized_choices.append([c[0],c[0]])
+                    normalized_choices.append([c[0], c[0]])
                 elif len(c) == 2:
                     normalized_choices.append(c)
     if int_keys:
         for c in normalized_choices:
             k = c[0]
-            if isinstance(k,str):
+            if isinstance(k, str):
                 try:
                     c[0] = int(k)
                 except ValueError:
                     pass
     return normalized_choices
 
 
@@ -54,21 +57,25 @@
         if val is None:
             setattr(obj, attr, {})
         else:
             setattr(obj, attr, copy.deepcopy(val))
 
 
 def pretty_format_querydict(qd):
-    out = ''
+    out = ""
     for k in sorted(qd.keys()):
         v = qd.getlist(k)
         if len(v) == 1:
             v = v[0]
-        out += "'{k}' : {v}\n".format(k=k,v=repr(v))
+        out += "'{k}' : {v}\n".format(k=k, v=repr(v))
     return out
 
 
+def is_ajax(request):
+    return request.META.get("HTTP_X_REQUESTED_WITH") == "XMLHttpRequest"
+
+
 class JsonDirect(str):
     pass
 
-#TODO : create functions to add sum/min/max/avg columns to a sequence
 
+# TODO : create functions to add sum/min/max/avg columns to a sequence
```

### Comparing `django-listing-0.0.9/django_listing/listing.py` & `django-listing-0.5.0/django_listing/listing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,191 @@
 #
 # Created : 2018-02-09
 #
 # @author: Eric Lapouyade
 #
 
-from django.utils.translation import ugettext as _
-from django.utils.translation import gettext_lazy, pgettext_lazy
-from django.utils.translation import to_locale
-from django.http import QueryDict
-from django.template import loader
+import collections
+import logging
+import pprint
+from urllib.parse import urlsplit, urlunsplit
+
+import tablib
+from django import forms
+from django.conf import settings
 from django.db.models import Model
 from django.db.models.query import QuerySet
-from django.conf import settings
-from django import forms
-from django.core.exceptions import ValidationError
-from django.forms.fields import FileField
+from django.http import QueryDict
 from django.middleware.csrf import get_token as get_csrf_token
-from urllib.parse import urlsplit, urlunsplit
+from django.template import loader
+from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy, pgettext_lazy
+
+from django_listing import EXPORT_FORMATS
 
-from .app_settings import app_settings
+from .columns import COLUMNS_PARAMS_KEYS, ModelColumns, SelectionColumn, SequenceColumns
+from .context import RenderContext
 from .exceptions import *
-from .record import RecordManager
+from .filters import FILTERS_PARAMS_KEYS, Filters
 from .html_attributes import HTMLAttributes
-from .context import RenderContext
-from .paginators import Paginator, PAGINATOR_PARAMS_KEYS
-from .columns import ( ModelColumns, SequenceColumns, COLUMNS_PARAMS_KEYS,
-                       SelectionColumn, )
-from .toolbar import Toolbar, TOOLBAR_PARAMS_KEYS
-from .filters import Filters, FILTERS_PARAMS_KEYS
+from .listing_form import LISTING_FORM_PARAMS_KEYS, ListingBaseForm
+from .paginators import PAGINATOR_PARAMS_KEYS, Paginator
+from .record import RecordManager
+from .theme_config import ThemeAttribute, ThemeTemplate
+from .toolbar import TOOLBAR_PARAMS_KEYS, Toolbar
 from .utils import init_dicts_from_class
-from .listing_form import ListingForm, LISTING_FORM_PARAMS_KEYS, ListingBaseForm
-from django_listing import EXPORT_FORMATS
-import tablib
-import collections
-import logging
-import pprint
-from copy import deepcopy
+
 pp = pprint.PrettyPrinter(indent=4)
 
-__all__ = ['ListingVariations', 'Listing', 'DivListing', 'logger']
+__all__ = ["ListingVariations", "Listing", "DivListing", "logger"]
 
-logger = logging.getLogger('django_listing')
+logger = logging.getLogger("django_listing")
 
 LISTING_ROWS_PER_PAGE = 20
 LISTING_ROWS_PER_PAGE_MAX = 500
-LISTING_SUFFIX_REQUEST_DATA_FIELD = '_listing_suffix_data'
-LISTING_SUFFIX_PATTERN = '_{}'
-LISTING_SELECTION_INPUT_NAME_KEY = 'selected_rows'
-LISTING_SELECTION_CHECKBOX_NAME = 'selection_checkbox'
-LISTING_SELECTION_HOVER_CSS_CLASS = 'hover'
-LISTING_SELECTOR_CSS_CLASS = 'row-selector'
+LISTING_SUFFIX_REQUEST_DATA_FIELD = "_listing_suffix_data"
+LISTING_SUFFIX_PATTERN = "-{}"
+LISTING_SELECTION_INPUT_NAME_KEY = "selected_rows"
+LISTING_SELECTION_CHECKBOX_NAME = "selection_checkbox"
+LISTING_SELECTION_HOVER_CSS_CLASS = "hover"
+LISTING_SELECTOR_CSS_CLASS = "row-selector"
 
 # only these parameters are allowed in the query string.
 LISTING_QUERY_STRING_KEYS = {
-    'sort','page','per_page','variation', 'select_columns', 'theme', 'export',
-    'editing_columns', 'editing_row_pk', 'editing', 'selecting'
-}
-LISTING_QUERY_STRING_INT_KEYS = {
-    'page','per_page','variation', 'editing_row_pk'
+    "editing",
+    "editing_columns",
+    "editing_row_pk",
+    "export",
+    "page",
+    "per_page",
+    "select_columns",
+    "selecting",
+    "sort",
+    "theme",
+    "variation",
 }
+LISTING_QUERY_STRING_INT_KEYS = {"page", "per_page", "variation", "editing_row_pk"}
 LISTING_NOT_PERSISTENT_QUERY_STRING_KEYS = set()
 
 # Only these attributes can be modified outside the class (in django templates,
 # views, listings instances ...)
 LISTING_PARAMS_KEYS = {
-    'sort','page','per_page', 'per_page_max', 'orphans', 'export', 'name',
-    'allow_empty_first_page', 'empty_table_msg', 'attrs',
-    'paginator_class', 'variation', 'suffix', 'div_rows', 'row_inner_div_tpl',
-    'variations', 'global_context','data', 'has_header',
-    'has_footer', 'has_paginator', 'select_columns', 'exclude_columns',
-    'theme_sort_asc_icon', 'theme_sort_desc_icon', 'theme_sort_none_icon',
-    'theme_sortable_class', 'theme_sort_asc_class', 'theme_sort_desc_class',
-    'columns_headers', 'theme', 'id', 'listing_template_name',
-    'div_row_template_name', 'toolbar', 'toolbar_placement', 'ajax_request',
-    'ajax_part', 'accept_ajax', 'div_template_name', 'sortable', 'unsortable',
-    'filters', 'theme_button_active_class', 'theme_button_disabled_class',
-    'empty_listing_template_name', 'record_label', 'footer_template_name',
-    'editable_columns', 'editing_columns', 'editing_row_pk', 'editable', 'editing',
-    'editing_hidden_columns', 'row_form_base_class', 'datetimepicker_date_format',
-    'datetimepicker_datetime_format', 'datetimepicker_time_format',
-    'save_to_database', 'primary_key', 'selectable', 'selecting',
-    'selection_multiple', 'selection_position', 'selection_key',
-    'row_attrs', 'theme_div_row_container_class', 'selection_mode',
-    'selection_overlay_template_name', 'selection_menu_id',
-    'onready_snippet','footer_snippet', 'selection_initial', 'form',
-    'link_object_columns', 'anchor_hash', 'theme_spinner_icon', 'has_upload',
-    'theme_action_button_class',
-    'theme_action_button_cancel_icon', 'theme_action_button_edit_icon',
-    'theme_action_button_update_icon', 'theme_action_button_upload_icon',
-    'action_button_cancel_label', 'action_button_edit_label',
-    'action_button_update_label', 'action_button_upload_label',
-    'action_footer_template_name', 'action_header_template_name',
-    'has_footer_action_buttons', 'edit_on_demand',
+    "accept_ajax",
+    "action_button_cancel_label",
+    "action_button_edit_label",
+    "action_button_update_label",
+    "action_button_upload_label",
+    "action_footer_template_name",
+    "action_header_template_name",
+    "ajax_part",
+    "ajax_request",
+    "allow_empty_first_page",
+    "anchor_hash",
+    "attrs",
+    "columns_headers",
+    "data",
+    "datetimepicker_date_format",
+    "datetimepicker_datetime_format",
+    "datetimepicker_time_format",
+    "div_row_template_name",
+    "div_rows",
+    "div_template_name",
+    "edit_on_demand",
+    "editable",
+    "editable_columns",
+    "editing",
+    "editing_columns",
+    "editing_hidden_columns",
+    "editing_row_pk",
+    "empty_listing_template_name",
+    "empty_table_msg",
+    "exclude_columns",
+    "export",
+    "filters",
+    "footer_snippet",
+    "footer_template_name",
+    "form",
+    "global_context",
+    "has_footer",
+    "has_footer_action_buttons",
+    "has_header",
+    "has_paginator",
+    "has_upload",
+    "id",
+    "is_small_device_localized",
+    "link_object_columns",
+    "listing_template_name",
+    "name",
+    "onready_snippet",
+    "orphans",
+    "page",
+    "paginator_class",
+    "per_page",
+    "per_page_max",
+    "primary_key",
+    "record_label",
+    "record_label_plural",
+    "row_attrs",
+    "row_form_base_class",
+    "row_inner_div_tpl",
+    "save_to_database",
+    "select_columns",
+    "selectable",
+    "selecting",
+    "selection_initial",
+    "selection_key",
+    "selection_menu_id",
+    "selection_mode",
+    "selection_multiple",
+    "selection_overlay_template_name",
+    "selection_position",
+    "small_device_header_style",
+    "small_device_max_width",
+    "sort",
+    "sortable",
+    "suffix",
+    "theme",
+    "theme_action_button_cancel_icon",
+    "theme_action_button_class",
+    "theme_action_button_edit_icon",
+    "theme_action_button_update_icon",
+    "theme_action_button_upload_icon",
+    "theme_button_active_class",
+    "theme_button_disabled_class",
+    "theme_div_row_container_class",
+    "theme_localized_small_device_styles_width",
+    "theme_sort_asc_class",
+    "theme_sort_asc_icon",
+    "theme_sort_desc_class",
+    "theme_sort_desc_icon",
+    "theme_sort_none_icon",
+    "theme_sortable_class",
+    "theme_sorted_class",
+    "theme_spinner_icon",
+    "toolbar",
+    "toolbar_placement",
+    "unsortable",
+    "use_datetimepicker",
+    "variation",
+    "variations",
 }
 
-LISTING_VARIATIONS_KEYS = LISTING_PARAMS_KEYS | {'get_url'}
-LISTING_FORMSET_PREFIX = 'listing'
+LISTING_VARIATIONS_KEYS = LISTING_PARAMS_KEYS | {"get_url"}
+LISTING_FORMSET_PREFIX = "listing"
 
 
 class ListingBase:
     def __init__(self, *args, **kwargs):
         self.stored_params = {}
         self.stored_columns_params = {}
         self.stored_toolbar_items_params = {}
         self.stored_filters_params = {}
         self.stored_form_params = {}
 
-    def transfert_params_from(self,listing):
+    def transfert_params_from(self, listing):
         self.stored_params = listing.stored_params
         self.stored_columns_params = listing.stored_columns_params
         self.stored_toolbar_items_params = listing.stored_toolbar_items_params
         self.stored_filters_params = listing.stored_filters_params
         self.stored_form_params = listing.stored_form_params
 
     def set_attr(self, attr, value):
@@ -118,74 +193,74 @@
 
     def store_kwargs(self, **kwargs):
         self.stored_params.update(kwargs)
 
     def store_html_attr(self, listing_attr, html_attr, value):
         html_params = self.stored_params.get(listing_attr)
         if html_params is None:
-            self.stored_params[listing_attr] = HTMLAttributes({html_attr:value})
+            self.stored_params[listing_attr] = HTMLAttributes({html_attr: value})
         else:
-            html_params.add(html_attr,value)
+            html_params.add(html_attr, value)
 
     def store_column_kwargs(self, name, **kwargs):
-        self.stored_columns_params.setdefault(name,{}).update(kwargs)
+        self.stored_columns_params.setdefault(name, {}).update(kwargs)
 
     def store_column_html_attr(self, name, col_attr, html_attr, value):
         col_params = self.stored_columns_params.get(name)
         if col_params is None:
-            param = {col_attr:HTMLAttributes({html_attr:value})}
-            self.store_column_kwargs(name,**param)
+            param = {col_attr: HTMLAttributes({html_attr: value})}
+            self.store_column_kwargs(name, **param)
         else:
-            html_params = col_params.setdefault(html_attr,HTMLAttributes())
-            html_params.add(html_attr,value)
+            html_params = col_params.setdefault(html_attr, HTMLAttributes())
+            html_params.add(html_attr, value)
 
     def store_toolbar_item_html_attr(self, name, tbi_attr, html_attr, value):
         tbi_params = self.stored_toolbar_items_params.get(name)
         if tbi_params is None:
-            param = {tbi_attr:HTMLAttributes({html_attr:value})}
-            self.store_toolbar_item_kwargs(name,**param)
+            param = {tbi_attr: HTMLAttributes({html_attr: value})}
+            self.store_toolbar_item_kwargs(name, **param)
         else:
-            html_params = tbi_params.setdefault(html_attr,HTMLAttributes())
-            html_params.add(html_attr,value)
+            html_params = tbi_params.setdefault(html_attr, HTMLAttributes())
+            html_params.add(html_attr, value)
 
     def get_column_kwargs(self, name):
         return self.stored_columns_params.get(name)
 
     def store_toolbar_item_kwargs(self, name, **kwargs):
-        self.stored_toolbar_items_params.setdefault(name,{}).update(kwargs)
+        self.stored_toolbar_items_params.setdefault(name, {}).update(kwargs)
 
     def get_toolbar_item_kwargs(self, name):
         return self.stored_toolbar_items_params.get(name)
 
     def store_filter_kwargs(self, name, **kwargs):
-        self.stored_filters_params.setdefault(name,{}).update(kwargs)
+        self.stored_filters_params.setdefault(name, {}).update(kwargs)
 
     def store_filter_html_attr(self, name, filter_attr, html_attr, value):
         filter_params = self.stored_filters_params.get(name)
         if filter_params is None:
-            param = {filter_attr:HTMLAttributes({html_attr:value})}
-            self.store_filter_kwargs(name,**param)
+            param = {filter_attr: HTMLAttributes({html_attr: value})}
+            self.store_filter_kwargs(name, **param)
         else:
-            html_params = filter_params.setdefault(html_attr,HTMLAttributes())
-            html_params.add(html_attr,value)
+            html_params = filter_params.setdefault(html_attr, HTMLAttributes())
+            html_params.add(html_attr, value)
 
     def get_filter_kwargs(self, name):
         return self.stored_filters_params.get(name)
 
     def store_form_kwargs(self, name, **kwargs):
-        self.stored_form_params.setdefault(name,{}).update(kwargs)
+        self.stored_form_params.setdefault(name, {}).update(kwargs)
 
     def store_form_html_attr(self, name, form_attr, html_attr, value):
         form_params = self.stored_form_params.get(name)
         if form_params is None:
-            param = {form_attr:HTMLAttributes({html_attr:value})}
-            self.store_form_kwargs(name,**param)
+            param = {form_attr: HTMLAttributes({html_attr: value})}
+            self.store_form_kwargs(name, **param)
         else:
-            html_params = form_params.setdefault(html_attr,HTMLAttributes())
-            html_params.add(html_attr,value)
+            html_params = form_params.setdefault(html_attr, HTMLAttributes())
+            html_params.add(html_attr, value)
 
     def get_form_kwargs(self, name):
         return self.stored_form_params.get(name)
 
 
 class ListingVariations(ListingBase):
     variations_classes = ()
@@ -217,15 +292,15 @@
             self.store_kwargs(**kwargs)
 
     def set_attr(self, attr, value):
         if self.listing:
             self.listing.set_attr(attr, value)
         else:
             # postpone to when listing will be created
-            self.store_kwargs(**{attr:value})
+            self.store_kwargs(**{attr: value})
 
     def is_initialized(self):
         if self.listing:
             return self.listing.is_initialized()
         else:
             return False
 
@@ -238,15 +313,15 @@
             self.store_kwargs(**kwargs)
 
     def create_listing(self, context):
         if not self.listing:
             request = context.request
             if self.suffix is None:
                 self.suffix = Listing.get_suffix(request, self)
-            variation = request.GET.get('variation'+self.suffix)
+            variation = request.GET.get("variation" + self.suffix)
             if variation and variation.isdigit():
                 variation = int(variation)
                 if variation >= len(self.variations_classes) or variation < 0:
                     variation = self.variation_default
             else:
                 variation = self.variation_default
 
@@ -255,16 +330,16 @@
             listing.variation = variation
             listing.variations = self
             listing.suffix = self.suffix
             listing.parsed_url = urlsplit(request.get_full_path())
             if self.id:
                 listing.id = self.id
             # Copy variations class attributes to listing instance
-            for k,v in self.__class__.__dict__.items():
-                if not k.startswith('_') and not getattr(listing,k,None):
+            for k, v in self.__class__.__dict__.items():
+                if not k.startswith("_") and not getattr(listing, k, None):
                     setattr(listing, k, v)
             listing.transfert_params_from(self)
             listing.set_kwargs()
             listing.init(self.data)
             self.listing = listing
 
     def render_init(self, context):
@@ -277,53 +352,58 @@
         self.listing.set_kwargs()
         return self.listing.render(context)
 
     def get_url(self, context, **kwargs):
         self.create_listing(context)
         return self.listing.get_url(context, **kwargs)
 
+    def have_to_refresh(self):
+        if self.listing:
+            return self.listing.have_to_refresh()
+        return False
+
     def __getattr__(self, item):
         if item in LISTING_VARIATIONS_KEYS and self.listing:
             return getattr(self.listing, item)
         return super().__getattribute__(item)
 
 
 class Listing(ListingBase):
     accept_ajax = False
     action = None
-    action_button_cancel_label = pgettext_lazy('action button','Cancel')
-    action_button_edit_label = pgettext_lazy('action button','Edit')
-    action_button_update_label = pgettext_lazy('action button','Update')
-    action_button_upload_label = pgettext_lazy('action button','Upload')
+    action_button_cancel_label = pgettext_lazy("action button", "Cancel")
+    action_button_edit_label = pgettext_lazy("action button", "Edit")
+    action_button_update_label = pgettext_lazy("action button", "Update")
+    action_button_upload_label = pgettext_lazy("action button", "Upload")
     action_col = None
-    action_footer_template_name = 'django_listing/action_footer.html'
-    action_header_template_name = 'django_listing/action_header.html'
+    action_footer_template_name = ThemeTemplate("action_footer.html")
+    action_header_template_name = ThemeTemplate("action_header.html")
     ajax_part = None
     allow_empty_first_page = True
     anchor_hash = None
-    attrs = {'class':'table table-hover table-bordered table-striped table-sm'}
+    attrs = {"class": "table table-hover table-bordered table-striped table-sm"}
     can_edit = False
     can_select = False
     columns = None
     columns_headers = None
     data = None
-    datetimepicker_date_format = 'Y-m-d'
-    datetimepicker_datetime_format = 'Y-m-d H:i'
-    datetimepicker_time_format = 'H:i'
-    div_template_name = 'django_listing/div_row.html'
-    row_attrs = {'class':'row-container'}
+    datetimepicker_date_format = "Y-m-d"
+    datetimepicker_datetime_format = "Y-m-d H:i"
+    datetimepicker_time_format = "H:i"
+    div_template_name = ThemeTemplate("div_row.html")
+    row_attrs = {}
     edit_on_demand = False
     editable = False
     editable_columns = set()
     editing = None
     editing_columns = None
     editing_row_pk = None
     editing_hidden_columns = None
-    empty_table_msg = gettext_lazy('Nothing to display')
-    empty_listing_template_name = 'django_listing/empty_listing.html'
+    empty_table_msg = gettext_lazy("Nothing to display")
+    empty_listing_template_name = ThemeTemplate("empty_listing.html")
     exclude_columns = None
     export = None
     filters = None
     footer_snippet = None
     footer_template_name = None
     form = None
     has_footer = False
@@ -331,91 +411,101 @@
     has_form = False
     has_header = True
     has_hidden_selection = False
     has_paginator = True
     has_toolbar = False
     has_upload = False
     id = None
+    is_small_device_localized = False
     link_object_columns = None
     row_form_base_class = ListingBaseForm
     listing_form_base_class = ListingBaseForm
-    listing_template_name = 'django_listing/listing.html'
+    listing_template_name = ThemeTemplate("listing.html")
     model = None
-    name = 'listing'
+    name = "listing"
     onready_snippet = None
     orphans = 0
     page = 1
     pagination = True
     paginator = None
     paginator_class = Paginator
     per_page = LISTING_ROWS_PER_PAGE
     per_page_max = LISTING_ROWS_PER_PAGE_MAX
     posted_columns = None
-    primary_key = 'id'
+    primary_key = "id"
     records_class = RecordManager
     record_label = None
+    record_label_plural = None
     row_form_errors = None
     row_inner_div_tpl = None
     save_to_database = False
     select_columns = None
     selectable = False
     selected_columns = None
     selected_hidden_columns = None
     selecting = None
     selection_initial = None
-    selection_key = 'id'
+    selection_key = "id"
     selection_menu_id = None
-    selection_mode = 'default'  # default, overlay, hover
+    selection_mode = "default"  # default, overlay, hover
     selection_multiple = False
-    selection_overlay_template_name = 'django_listing/selection_overlay.html'
-    selection_position = 'hidden'  # left, right or hidden
+    selection_overlay_template_name = ThemeTemplate("selection_overlay.html")
+    selection_position = "hidden"  # left, right or hidden
+    small_device_max_width = "767.98px"
+    small_device_header_style = "font-weight: bold"
     sort = None
     sortable = True
     suffix = None
-    theme = 'standard-theme'
     toolbar = None
-    toolbar_placement = 'both'
+    toolbar_placement = "both"
     unsortable = True
+    use_datetimepicker = False
     variation = None
     variations = None
 
     params_keys = set()  # keep it here in the class not in __init__()
 
-    theme_listing_class = 'django-listing'
-    theme_action_button_class = 'btn btn-primary'
-    theme_action_button_cancel_icon = ''
-    theme_action_button_edit_icon = ''
-    theme_action_button_update_icon = ''
-    theme_action_button_upload_icon = ''
-    theme_container_class = 'django-listing-container'
-    theme_sort_asc_icon = 'listing-icon-angle-up'
-    theme_sort_desc_icon = 'listing-icon-angle-down'
-    theme_sort_none_icon = ''
-    theme_spinner_icon = 'animate-spin listing-icon-spin2'
-    theme_sortable_class = 'sortable'
-    theme_sort_asc_class = 'asc'
-    theme_sort_desc_class = 'desc'
-    theme_button_class = 'btn btn-primary'
-    theme_button_disabled_class = 'disabled'
-    theme_button_active_class = 'active'
-    theme_div_row_container_class = ''
+    theme_class = ThemeAttribute("theme_class")
+    theme_listing_class = ThemeAttribute("theme_listing_class")
+    theme_action_button_class = ThemeAttribute("theme_action_button_class")
+    theme_action_button_cancel_icon = ThemeAttribute("theme_action_button_cancel_icon")
+    theme_action_button_edit_icon = ThemeAttribute("theme_action_button_edit_icon")
+    theme_action_button_update_icon = ThemeAttribute("theme_action_button_update_icon")
+    theme_action_button_upload_icon = ThemeAttribute("theme_action_button_upload_icon")
+    theme_container_class = ThemeAttribute("theme_container_class")
+    theme_sort_asc_icon = ThemeAttribute("theme_sort_asc_icon")
+    theme_sort_desc_icon = ThemeAttribute("theme_sort_desc_icon")
+    theme_sort_none_icon = ThemeAttribute("theme_sort_none_icon")
+    theme_spinner_icon = ThemeAttribute("theme_spinner_icon")
+    theme_sortable_class = ThemeAttribute("theme_sortable_class")
+    theme_sorted_class = ThemeAttribute("theme_sorted_class")
+    theme_sort_asc_class = ThemeAttribute("theme_sort_asc_class")
+    theme_sort_desc_class = ThemeAttribute("theme_sort_desc_class")
+    theme_button_class = ThemeAttribute("theme_button_class")
+    theme_button_disabled_class = ThemeAttribute("theme_button_disabled_class")
+    theme_button_active_class = ThemeAttribute("theme_button_active_class")
+    theme_div_row_container_class = ThemeAttribute("theme_div_row_container_class")
+    theme_row_class = ThemeAttribute("theme_row_class")
+    theme_localized_small_device_styles_width = ThemeAttribute(
+        "theme_localized_small_device_styles_width"
+    )
 
     def __init__(self, data=None, **kwargs):
-        super().__init__(data,**kwargs)
+        super().__init__(data, **kwargs)
         self.request = None
         self.parsed_url = None
         self.page_context = None
         self.records = self.records_class(self)
         self.rows_context_list = []
         self.form_input_hiddens = []
         self.editing_hidden_form_fields = []
         self.editing_really_hidden_columns = set()
         self.can_edit_columns = []
         self.col_cell_renderers = {}
-        init_dicts_from_class(self,['global_context','attrs','row_attrs'])
+        init_dicts_from_class(self, ["global_context", "attrs", "row_attrs"])
         self._initialized = False
         self._render_initialized = False
         self._formset = None
         self._view = None
         self.form_params = {}
         self._have_to_refresh = False
 
@@ -425,109 +515,114 @@
         if isinstance(data, QuerySet) or data is not None:
             self.init(data, **kwargs)
 
     @classmethod
     def get_params_keys(cls):
         if not Listing.params_keys:
             Listing.params_keys = set(LISTING_PARAMS_KEYS)
+            Listing.params_keys.update({"columns_%s" % k for k in COLUMNS_PARAMS_KEYS})
             Listing.params_keys.update(
-                {'columns_%s' % k for k in COLUMNS_PARAMS_KEYS})
-            Listing.params_keys.update(
-                {'paginator_%s' % k for k in PAGINATOR_PARAMS_KEYS})
-            Listing.params_keys.update(
-                {'toolbar_%s' % k for k in TOOLBAR_PARAMS_KEYS})
-            Listing.params_keys.update(
-                {'filters_%s' % k for k in FILTERS_PARAMS_KEYS})
+                {"paginator_%s" % k for k in PAGINATOR_PARAMS_KEYS}
+            )
+            Listing.params_keys.update({"toolbar_%s" % k for k in TOOLBAR_PARAMS_KEYS})
+            Listing.params_keys.update({"filters_%s" % k for k in FILTERS_PARAMS_KEYS})
             Listing.params_keys.update(
-                {'form_%s' % k for k in LISTING_FORM_PARAMS_KEYS})
+                {"form_%s" % k for k in LISTING_FORM_PARAMS_KEYS}
+            )
         return Listing.params_keys
 
     def set_kwargs(self, **kwargs):
         self.store_kwargs(**kwargs)
         params_keys = self.get_params_keys()
         for k, v in self.stored_params.items():
-            if k in params_keys or ('__' in k and not k.startswith('__')):
-                setattr(self,k,v)
+            if k in params_keys or ("__" in k and not k.startswith("__")):
+                setattr(self, k, v)
         self.stored_params = {}
 
     def have_to_refresh(self):
         return self._have_to_refresh
 
     def plan_refresh(self):
         self._have_to_refresh = True
 
     def add_onready_snippet(self, snippet):
-        if not hasattr(self.request,'django_listing_onready_snippets'):
+        if not hasattr(self.request, "django_listing_onready_snippets"):
             self.request.django_listing_onready_snippets = []
         if snippet not in self.request.django_listing_onready_snippets:
             self.request.django_listing_onready_snippets.append(snippet)
 
     def add_header_snippet(self, snippet):
-        if not hasattr(self.request,'django_listing_header_snippets'):
+        if not hasattr(self.request, "django_listing_header_snippets"):
             self.request.django_listing_header_snippets = []
         if snippet not in self.request.django_listing_header_snippets:
             self.request.django_listing_header_snippets.append(snippet)
 
     def add_footer_dict_list(self, key, dct):
-        if not hasattr(self.request,'django_listing_footer_dict_list'):
+        if not hasattr(self.request, "django_listing_footer_dict_list"):
             self.request.django_listing_footer_dict_list = {}
         dict_list = self.request.django_listing_footer_dict_list.setdefault(key, [])
         dict_list.append(dct)
 
     def add_footer_snippet(self, snippet):
-        if not hasattr(self.request,'django_listing_footer_snippets'):
+        if not hasattr(self.request, "django_listing_footer_snippets"):
             self.request.django_listing_footer_snippets = []
         if snippet not in self.request.django_listing_footer_snippets:
             self.request.django_listing_footer_snippets.append(snippet)
 
     def need_media_for(self, feature_name):
-        if not hasattr(self.request, 'need_media_for'):
+        if not hasattr(self.request, "need_media_for"):
             self.request.need_media_for = {}
         self.request.need_media_for[feature_name] = True
 
     def create_missing_columns(self):
         if self.columns is None:
-            if isinstance(self.columns_headers,str):
-                self.columns_headers = self.columns_headers.split(',')
+            if isinstance(self.columns_headers, str):
+                self.columns_headers = self.columns_headers.split(",")
             if self.model:
                 self.columns = ModelColumns(
-                    self.model, listing=self,
-                    link_object_columns=self.link_object_columns )
-            elif self.data and isinstance(self.data,collections.Sequence):
-                self.columns = SequenceColumns(self.data, self.columns_headers,
-                                               listing=self)
-        if not self.columns:
-            raise InvalidListing(_('Please configure at least one column '
-                                   'in your listing'))
-        if self.selectable:
-            if self.selection_position == 'left':
-                self.columns.insert(
-                    0,
-                    SelectionColumn(LISTING_SELECTION_CHECKBOX_NAME)
+                    self.model,
+                    listing=self,
+                    link_object_columns=self.link_object_columns,
                 )
-            elif self.selection_position == 'right':
-                self.columns.append(
-                    SelectionColumn(LISTING_SELECTION_CHECKBOX_NAME)
+            elif self.data and isinstance(self.data, collections.abc.Sequence):
+                self.columns = SequenceColumns(
+                    self.data, self.columns_headers, listing=self
                 )
+        if isinstance(self.columns, (ModelColumns, SequenceColumns)):
+            self.columns.set_listing(self)
+            self.columns.init()
+        if not self.columns:
+            raise InvalidListing(
+                _("Please configure at least one column " "in your listing")
+            )
+        if self.selectable:
+            if self.selection_position == "left":
+                self.columns.insert(0, SelectionColumn(LISTING_SELECTION_CHECKBOX_NAME))
+            elif self.selection_position == "right":
+                self.columns.append(SelectionColumn(LISTING_SELECTION_CHECKBOX_NAME))
 
     def create_missing_toolbar_items(self):
         if self.toolbar is None:
             return
-        if not isinstance(self,Toolbar):
+        if not isinstance(self, Toolbar):
             self.toolbar = Toolbar(self.toolbar)
 
     def create_missing_filters(self):
         if self.filters is None:
             return
-        if isinstance(self.filters,str):
+        if isinstance(self.filters, str):
             # if filters attribute is a string, it means a layout was declared,
             # so we have to extract filters names
             form_layout = self.filters
-            filters_name = list(map(lambda s:s.split('|')[0].strip(),
-                sum(map(lambda s:s.split(','),form_layout.split(';')),[])))
+            filters_name = list(
+                map(
+                    lambda s: s.split("|")[0].strip(),
+                    sum(map(lambda s: s.split(","), form_layout.split(";")), []),
+                )
+            )
             self.filters = Filters(*filters_name)
             self.filters.form_layout = form_layout
 
     def get_model(self):
         if self.model:
             return self.model
         if self.columns:
@@ -552,157 +647,189 @@
                 self.suffix = self.get_suffix(self.request, self)
                 self.extract_params()
                 if self.filters:
                     self.filters.extract_params()
             else:
                 self.page_context = context
 
+    def validate_parameters(self):
+        if self.editable and self.accept_ajax:
+            if self.row_form_errors is None:
+                self.row_form_errors = []
+            self.row_form_errors.append(_("[CANNOT_EDIT_IN_AJAX]"))
+            self.editable = False
+
     def init(self, data, context=None, **kwargs):
         if not self.is_initialized():
             self.set_kwargs(**kwargs)
+            self.validate_parameters()
             if data is None:
                 data = self.model or self.columns.get_model()
-            if isinstance(data,type) and issubclass(data, Model):
+            if isinstance(data, type) and issubclass(data, Model):
                 self.model = data
                 data = self.model.objects.all()
-            elif isinstance(data,Model):
+            elif isinstance(data, Model):
                 self.model = type(data)
                 data = self.model.objects.all()
-            elif isinstance(data,QuerySet):
+            elif isinstance(data, QuerySet):
                 self.model = data.model
             if self.record_label is None:
                 if self.model:
-                    self.record_label = self.model.__name__.lower()
+                    self.record_label = self.model._meta.verbose_name
                 else:
-                    self.record_label = _('record')
+                    self.record_label = _("record")
+            if self.record_label_plural is None:
+                if self.model:
+                    self.record_label_plural = self.model._meta.verbose_name_plural
+                else:
+                    self.record_label_plural = _("records")
             self.data = data
             self.create_missing_filters()
             if self.filters:
                 self.filters = self.filters.bind_to_listing(self)
             if self.form:
                 self.form = self.form.bind_to_listing(self)
             self.manage_page_context(context)
             self.create_missing_columns()
             self.create_missing_toolbar_items()
             self.has_toolbar = bool(self.toolbar)
             self.columns = self.columns.bind_to_listing(self)
             if self.toolbar:
                 self.toolbar = self.toolbar.bind_to_listing(self)
             self.col_cell_renderers = {
-                col : getattr(self, 'render_{}'.format(col.name), col.render_cell)
-                for col in self.columns }
+                col: getattr(self, "render_{}".format(col.name), col.render_cell)
+                for col in self.columns
+            }
             self._initialized = True
 
     def datetimepicker_init(self):
-        self.need_media_for('datetimepicker')
-        self.add_footer_dict_list('datetimepickers', dict(
-            listing=self,
-            div_id=self.id
-        ))
+        if self.use_datetimepicker:
+            self.need_media_for("datetimepicker")
+            self.add_footer_dict_list(
+                "datetimepickers", dict(listing=self, div_id=self.id)
+            )
 
     def dropzone_init(self):
-        self.need_media_for('dropzone')
-        dz_suffix = self.suffix[1:] if isinstance(self.suffix, str) else ''
-        dz_camel_name = f'actionForm{dz_suffix}'
-        self.add_footer_dict_list('dropzones', dict(
-            listing=self,
-            dz_camel_name=dz_camel_name,
-            options=app_settings.DROPZONE_PARAMS,
-        ))
+        self.need_media_for("dropzone")
+        dz_suffix = self.suffix[1:] if isinstance(self.suffix, str) else ""
+        dz_camel_name = f"actionForm{dz_suffix}"
+        self.add_footer_dict_list(
+            "dropzones",
+            dict(
+                listing=self,
+                dz_camel_name=dz_camel_name,
+                options=settings.django_listing_settings.DROPZONE_PARAMS,
+            ),
+        )
 
     def global_context_init(self):
-        self.global_context.update(app_settings.context)
-        if self.request and ( self.can_edit or self.has_upload ):
-            self.global_context['csrf_token'] = get_csrf_token(self.request)
+        self.global_context.update(settings.django_listing_settings.context)
+        if self.request and (self.can_edit or self.has_upload):
+            self.global_context["csrf_token"] = get_csrf_token(self.request)
 
-    def render_init(self,context):
+    def render_init(self, context):
         if not self._render_initialized:
             self.manage_page_context(context)
             self.normalize_params()
             for col in self.columns:
                 col.render_init()
             if isinstance(self.editable_columns, str):
                 self.editable_columns = set(
-                    map(str.strip, self.editable_columns.split(',')))
+                    map(str.strip, self.editable_columns.split(","))
+                )
             if self.editing_hidden_columns is None:
                 if self.model and self.primary_key in self.columns.names():
                     self.editing_hidden_columns = {self.primary_key}
                 else:
                     self.editing_hidden_columns = set()
             if isinstance(self.editing_hidden_columns, str):
                 self.editing_hidden_columns = set(
-                    map(str.strip, self.editing_hidden_columns.split(',')))
+                    map(str.strip, self.editing_hidden_columns.split(","))
+                )
             if self.editing is None:
                 self.editing = True
             if self.editing_columns is None:
-                self.editing_columns = 'all'
-            if isinstance(self.editing, str) and self.editing.lower() == 'false':
+                self.editing_columns = "all"
+            if isinstance(self.editing, str) and self.editing.lower() == "false":
                 self.editing = False
             if isinstance(self.editing_columns, str):
                 self.editing_columns = set(
-                    map(str.strip, self.editing_columns.split(',')))
+                    map(str.strip, self.editing_columns.split(","))
+                )
             self.columns.editing_init()
             self.can_edit = self.editable and self.editing
-            if ( isinstance(self.selecting, str) and
-                 self.selecting.lower() == 'false' ):
+            if isinstance(self.selecting, str) and self.selecting.lower() == "false":
                 self.selecting = False
             if self.selecting is None:
                 self.selecting = True
             self.can_select = self.selectable and self.selecting
-            self.has_hidden_selection = ( self.selectable and
-                                          self.selecting and
-                                          self.selection_position == 'hidden')
+            self.has_hidden_selection = (
+                self.selectable
+                and self.selecting
+                and self.selection_position == "hidden"
+            )
             is_exporting = self.export_data()
             if is_exporting:
-                return 'Sending listing export file...'
+                return "Sending listing export file..."
             self.columns_sort_ascending = {}
             self.columns_sort_list = []
             if self.sort:
-                for col_name in map(str.strip,self.sort.split(',')):
+                if isinstance(self.sort, str):
+                    sort_list = map(str.strip, self.sort.split(","))
+                else:
+                    sort_list = self.sort
+                for col_name in sort_list:
                     ascending = True
-                    if col_name.startswith('-'):
+                    if col_name.startswith("-"):
                         col_name = col_name[1:]
                         ascending = False
                     self.columns_sort_list.append(col_name)
                     self.columns_sort_ascending[col_name] = ascending
-            if not isinstance(self.attrs,HTMLAttributes):
+            if not isinstance(self.attrs, HTMLAttributes):
                 self.attrs = HTMLAttributes(self.attrs)
-            html_class = 'listing-'+self.__class__.__name__.lower()
-            self.attrs.add('class',{ html_class, self.theme_listing_class })
+            html_class = "listing-" + self.__class__.__name__.lower()
+            self.attrs.add("class", {html_class, self.theme_listing_class})
             if self.variation is not None:
-                self.attrs.add('class','variation-{}'.format(self.variation))
+                self.attrs.add("class", "variation-{}".format(self.variation))
             if not self.id:
-                self.id = '{}{}-id'.format(html_class,self.suffix)
-            if not isinstance(self.row_attrs,HTMLAttributes):
-                self.row_attrs = HTMLAttributes(
-                    self.row_attrs )
+                self.id = "{}{}-id".format(html_class, self.suffix)
+            self.css_id = self.id.replace("_", "-")
+            if isinstance(self.suffix, str):
+                self.css_suffix = self.suffix.replace("_", "-")
+            if not isinstance(self.row_attrs, HTMLAttributes):
+                self.row_attrs = HTMLAttributes(self.row_attrs)
             self.row_attrs.add(
-                'class',{ self.theme_div_row_container_class })
-            self.selected_columns = self.columns.select(self.select_columns,
-                                                        self.exclude_columns)
-            self.can_edit_columns=[ c for c in self.selected_columns if c.can_edit ]
-            self.can_edit_columns_names=set( c.name for c in self.can_edit_columns )
-            self.editing_really_hidden_columns = \
+                "class", {self.theme_div_row_container_class, self.theme_row_class}
+            )
+            self.selected_columns = self.columns.select(
+                self.select_columns, self.exclude_columns
+            )
+            self.can_edit_columns = [c for c in self.selected_columns if c.can_edit]
+            self.can_edit_columns_names = set(c.name for c in self.can_edit_columns)
+            self.editing_really_hidden_columns = (
                 self.editing_hidden_columns - self.can_edit_columns_names
-            self.selected_hidden_columns = \
-                self.columns.select(self.editing_really_hidden_columns)
+            )
+            self.selected_hidden_columns = self.columns.select(
+                self.editing_really_hidden_columns
+            )
             if self.can_edit:
                 self.datetimepicker_init()
             if self.has_upload:
                 self.dropzone_init()
             if self.can_edit or self.can_select or self.form or self.has_upload:
-                self.add_form_input_hiddens(listing_id=self.id,
-                                            listing_suffix=self.suffix)
+                self.add_form_input_hiddens(
+                    listing_id=self.id, listing_suffix=self.suffix
+                )
             if self.onready_snippet:
                 self.add_onready_snippet(self.onready_snippet)
             if self.footer_snippet:
                 self.add_footer_snippet(self.footer_snippet)
-            if not isinstance(self.selection_initial,list):
+            if not isinstance(self.selection_initial, list):
                 self.selection_initial = [self.selection_initial]
-            self.selection_has_overlay = self.selection_mode in ['overlay', 'hover']
+            self.selection_has_overlay = self.selection_mode in ["overlay", "hover"]
             self.global_context_init()
             self.records.compute_current_page_records()
             self._render_initialized = True
 
     def render(self, context):
         response = self.render_init(context)
         if response is not None:
@@ -710,73 +837,84 @@
         return self.render_template()
 
     def export_data(self):
         if self.export:
             export_format = self.export.upper()
             if export_format in EXPORT_FORMATS:
                 headers = self.exported_headers()
-                if export_format == 'DBF':
-                    headers = list(map(lambda h:h[:10],headers))
+                if export_format == "DBF":
+                    headers = list(map(lambda h: h[:10], headers))
                 data = tablib.Dataset()
                 data.headers = headers
                 for row in self.exported_rows():
                     data.append(row)
                 self.request.export_data = data.export(export_format.lower())
-                self.request.export_filename = '{}.{}'.format(self.name,
-                                                          self.export.lower())
-        return hasattr(self.request,'export_data')
+                self.request.export_filename = "{}.{}".format(
+                    self.name, self.export.lower()
+                )
+        return hasattr(self.request, "export_data")
 
     def django_listing_info(self):
-        if hasattr(self, 'request'):
-            if self.request.GET.get('__django_listing_info__'):
-                out = '<b><u>django-listing informations :</u></b><br>'
+        if hasattr(self, "request"):
+            if self.request.GET.get("__django_listing_info__"):
+                out = "<b><u>django-listing informations :</u></b><br>"
                 import django_listing
-                out += f'django-listing version : {django_listing.__version__}<br>'
+
+                out += f"django-listing version : {django_listing.__version__}<br>"
                 import django
-                out += f'django version : {django.__version__}<br>'
+
+                out += f"django version : {django.__version__}<br>"
                 import tablib
-                out += f'tablib version : {tablib.__version__}<br>'
+
+                out += f"tablib version : {tablib.__version__}<br>"
                 import sys
-                out += f'Python version : {sys.version.split()[0]}<br>'
+
+                out += f"Python version : {sys.version.split()[0]}<br>"
                 return out
 
     def render_template(self):
         request_for_info = self.django_listing_info()
         if request_for_info:
             return request_for_info
         ctx = self.get_listing_context()
         template = loader.get_template(self.listing_template_name)
         out = template.render(ctx)
         return out
 
+    def get_listing_css_id(self):
+        return str(self.id).replace("_", "-")
+
     def get_listing_context(self):
-        has_top_toolbar = ( self.has_toolbar and
-                            self.toolbar_placement in ['top','both'] )
-        has_bottom_toolbar = ( self.has_toolbar and
-                               self.toolbar_placement in ['bottom','both'] )
-        listing_container_class = '{} {}'.format(
-            self.theme_container_class, self.theme)
+        has_top_toolbar = self.has_toolbar and self.toolbar_placement in ["top", "both"]
+        has_bottom_toolbar = self.has_toolbar and self.toolbar_placement in [
+            "bottom",
+            "both",
+        ]
+        listing_container_class = "{} {}".format(
+            self.theme_container_class, self.theme_class
+        )
         if self.accept_ajax:
-            listing_container_class += ' django-listing-ajax'
+            listing_container_class += " django-listing-ajax"
         if self.can_edit:
-            listing_container_class += ' django-listing-editing'
+            listing_container_class += " django-listing-editing"
         if self.can_select:
-            listing_container_class += ' django-listing-selecting'
+            listing_container_class += " django-listing-selecting"
             if self.selection_multiple:
-                listing_container_class += ' selection_multiple'
+                listing_container_class += " selection_multiple"
             else:
-                listing_container_class += ' selection_unique'
-            listing_container_class += \
-                ' selection_position_{}'.format(self.selection_position)
+                listing_container_class += " selection_unique"
+            listing_container_class += " selection_position_{}".format(
+                self.selection_position
+            )
         if self.has_upload:
-            listing_container_class += ' has_upload'
-        sel_css_class = ( LISTING_SELECTOR_CSS_CLASS
-                          if self.selection_has_overlay else '' )
-        hover_css_class = ( LISTING_SELECTION_HOVER_CSS_CLASS
-                          if self.selection_mode == 'hover' else '' )
+            listing_container_class += " has_upload"
+        sel_css_class = LISTING_SELECTOR_CSS_CLASS if self.selection_has_overlay else ""
+        hover_css_class = (
+            LISTING_SELECTION_HOVER_CSS_CLASS if self.selection_mode == "hover" else ""
+        )
         ctx = RenderContext(
             self.global_context,
             self.page_context.flatten(),
             nb_columns=len(self.selected_columns),
             listing=self,
             listing_container_class=listing_container_class,
             has_top_toolbar=has_top_toolbar,
@@ -788,21 +926,21 @@
         if self.paginator:
             ctx.update(self.paginator.get_context())
         if self.toolbar:
             ctx.update(self.toolbar.get_context())
         return ctx
 
     def add_form_input_hiddens(self, **kwargs):
-        for name,value in kwargs.items():
-            self.form_input_hiddens.append((name,value))
+        for name, value in kwargs.items():
+            self.form_input_hiddens.append((name, value))
 
-    def add_edit_form_hidden_field(self,field_instance):
+    def add_edit_form_hidden_field(self, field_instance):
         self.editing_hidden_form_fields.append(field_instance)
 
-    def aggregate(self,rec):
+    def aggregate(self, rec):
         for col in self.selected_columns:
             if col.aggregation:
                 col.aggregation.aggregate(rec)
 
         if self.can_edit:
             for col in self.selected_hidden_columns:
                 form = rec.get_form()
@@ -841,19 +979,19 @@
             )
             if self.has_hidden_selection:
                 row.update(selection_value=rec.get(self.selection_key))
             self.aggregate(rec)
             yield row
 
     def exported_headers(self):
-        return [ str(c.get_header_value()) for c in self.columns ]
+        return [str(c.get_header_value()) for c in self.columns]
 
     def exported_rows(self):
         for rec in self.records.export():
-            yield [ c.get_cell_exported_value(rec) for c in self.columns ]
+            yield [c.get_cell_exported_value(rec) for c in self.columns]
 
     def get_rendered_cells(self, rec):
         rendered_columns = []
         for col in self.selected_columns:
             rendered_col = dict(
                 html=self.col_cell_renderers[col](rec),
                 obj=col,
@@ -870,106 +1008,136 @@
                     obj=col,
                 )
                 rendered_columns.append(rendered_col)
             return rendered_columns
         else:
             return []
 
+    def get_localized_small_device_styles(self):
+        styles = [
+            ("#{listing_css_id} th:before {{" 'content:"{sort_msg}";' "}}").format(
+                listing_css_id=self.get_listing_css_id(),
+                sort_msg=_("Sort by:"),
+                two_dots=_(":"),
+            )
+        ]
+        for col in self.selected_columns:
+            style = (
+                "#{listing_css_id} td.col-{col_name}:before {{"
+                'content:"{header}{two_dots} ";'
+                "{sd_style};"
+                "}}"
+            ).format(
+                listing_css_id=self.get_listing_css_id(),
+                col_name=col.name,
+                header=col.get_header_value(),
+                two_dots=_(":"),
+                sd_style=self.small_device_header_style,
+            )
+            styles.append(style)
+        return styles
+
     def footer_columns(self):
         if self.has_footer:
             rendered_columns = []
             for col in self.selected_columns:
                 rendered_col = dict(
                     html=col.render_footer(),
                     obj=col,
                 )
                 rendered_columns.append(rendered_col)
             return rendered_columns
         else:
             return []
 
     def get_url(self, context=None, without=None, anchor_hash=None, **kwargs):
-        """ Get listing url with some updated parameters if needed
+        """Get listing url with some updated parameters if needed
         Note : Do not remove 'context=None' because needed by listing variations
         """
         querystring = QueryDict(self.parsed_url.query, mutable=True)
-        for k,v in kwargs.items():
-            if not isinstance(v,str):
+        for k, v in kwargs.items():
+            if not isinstance(v, str):
                 v = str(v)
             if k in LISTING_QUERY_STRING_KEYS:
                 k += self.suffix
             querystring[k] = v
         del_keys = LISTING_NOT_PERSISTENT_QUERY_STRING_KEYS - set(kwargs.keys())
         if without:
-            if isinstance(without,str):
-                without=without.split(',')
+            if isinstance(without, str):
+                without = without.split(",")
             del_keys = del_keys | set(without)
         for k in del_keys:
             k += self.suffix
             if k in querystring:
                 del querystring[k]
         fragment = anchor_hash or self.anchor_hash
-        return urlunsplit(self.parsed_url._replace(
-                            query=querystring.urlencode(),
-                            fragment=fragment))
+        return urlunsplit(
+            self.parsed_url._replace(query=querystring.urlencode(), fragment=fragment)
+        )
 
     def get_hiddens(self, without=None):
         hiddens = QueryDict(self.parsed_url.query, mutable=True)
         if without:
-            if isinstance(without,str):
-                without = list(map(str.strip,without.split(',')))
-            without = list(map(lambda s:s.strip()+self.suffix,without))
-            if isinstance(without,(list,tuple)):
+            if isinstance(without, str):
+                without = list(map(str.strip, without.split(",")))
+            without = list(map(lambda s: s.strip() + self.suffix, without))
+            if isinstance(without, (list, tuple)):
                 for k in without:
                     if k in hiddens:
                         del hiddens[k]
         return hiddens
 
     def get_hiddens_html(self, without=None):
         hiddens = self.get_hiddens(without)
-        out = ['<input type="hidden" name="{name}" value="{value}">'.format(
-            name=name,
-            value=value
-        ) for name, value in hiddens.items()]
-        return ''.join(out)
+        out = [
+            '<input type="hidden" name="{name}" value="{value}">'.format(
+                name=name, value=value
+            )
+            for name, value in hiddens.items()
+        ]
+        return "".join(out)
 
     @classmethod
     def get_suffix_request_data(cls, request):
         if not hasattr(request, LISTING_SUFFIX_REQUEST_DATA_FIELD):
-            setattr(request,LISTING_SUFFIX_REQUEST_DATA_FIELD, {
-                'listings_suffixes' : {},
-                'counter' : 0,
-            })
-        return getattr(request,LISTING_SUFFIX_REQUEST_DATA_FIELD)
+            setattr(
+                request,
+                LISTING_SUFFIX_REQUEST_DATA_FIELD,
+                {
+                    "listings_suffixes": {},
+                    "counter": 0,
+                },
+            )
+        return getattr(request, LISTING_SUFFIX_REQUEST_DATA_FIELD)
 
     @classmethod
     def get_suffix(cls, request, listing):
-        listing = getattr(listing,'variations',None) or listing
+        listing = getattr(listing, "variations", None) or listing
         data = cls.get_suffix_request_data(request)
-        suffix = data['listings_suffixes'].get(listing)
+        suffix = data["listings_suffixes"].get(listing)
         if suffix is None:
-            counter = data['counter']
-            suffixes = data['listings_suffixes'].values()
+            counter = data["counter"]
+            suffixes = data["listings_suffixes"].values()
             while True:
                 if counter == 0:
-                    suffix = ''
+                    suffix = ""
                 else:
                     suffix = LISTING_SUFFIX_PATTERN.format(counter)
                 if suffix not in suffixes:
-                    data['listings_suffixes'][listing] = suffix
+                    data["listings_suffixes"][listing] = suffix
                     break
                 counter += 1
-            data['counter'] = counter + 1
+            data["counter"] = counter + 1
         return suffix
 
     @classmethod
     def set_suffix(cls, request, listing, suffix):
-        listing = getattr(listing,'variations',None) or listing
+        listing = getattr(listing, "variations", None) or listing
         data = cls.get_suffix_request_data(request)
-        data['listings_suffixes'][listing] = suffix
+        data["listings_suffixes"][listing] = suffix
         listing.suffix = suffix
 
     def extract_params(self):
         get_dict = self.request.GET
         post_dict = self.request.POST
         for k in LISTING_QUERY_STRING_KEYS:
             qs_key = k + self.suffix
@@ -986,71 +1154,84 @@
             if v is not None:
                 setattr(self, k, v)
 
     def normalize_params(self):
         if self.per_page < -1 or self.per_page == 0:
             self.per_page = self.__class__.per_page
 
-    def get_row_attrs(self,rec):
+    def get_row_attrs(self, rec):
         attrs = HTMLAttributes(self.row_attrs)  # create a copy
         if rec.pk:
-            attrs.add('data-pk',str(rec.pk))
-        attrs.add('class','odd' if rec.get_index() % 2 else 'even')
+            attrs.add("data-pk", str(rec.pk))
+        attrs.add("class", "odd" if rec.get_index() % 2 else "even")
         if self.can_select:
             if not self.selection_has_overlay:
-                attrs.add('class',LISTING_SELECTOR_CSS_CLASS)
+                attrs.add("class", LISTING_SELECTOR_CSS_CLASS)
             selection_value = rec.get(self.selection_key)
             if self.selection_initial and selection_value in self.selection_initial:
-                attrs.add('class', 'selected')
+                attrs.add("class", "selected")
                 rec._selected = True
         return attrs
 
     def get_row_context(self, rec):
         return {}
 
     def get_formset_initial_values(self):
-        return [ {c.name:c.get_cell_value(rec)
-                 for c in (self.can_edit_columns+self.selected_hidden_columns)}
-                 for rec in self.records.current_page()
-                 if not self.editing_row_pk or rec.pk == self.editing_row_pk
-               ]
+        initial_values = [
+            {
+                c.name: c.get_cell_form_value(rec)
+                for c in (self.can_edit_columns + self.selected_hidden_columns)
+            }
+            for rec in self.records.current_page()
+            if not self.editing_row_pk or rec.pk == self.editing_row_pk
+        ]
+        return initial_values
 
     def get_formset(self):
         if not self._formset:
             post_data = None
             post_files = None
-            if self.request.method == 'POST':
-                posted_listing_id = self.request.POST.get('listing_id', '')
+            if self.request.method == "POST":
+                posted_listing_id = self.request.POST.get("listing_id", "")
                 if posted_listing_id == self.id:
                     post_data = self.request.POST
                     post_files = self.request.FILES
-            fields = { c.name : c.create_hidden_form_field()
-                            for c in self.selected_hidden_columns }
-            fields.update({ c.name : c.create_form_field()
-                       for c in self.can_edit_columns })
-            form_class = type('ListingRowForm{}'.format(self.suffix),
-                              (self.row_form_base_class,),
-                              {'base_fields': fields})
+            fields = {
+                c.name: c.create_hidden_form_field()
+                for c in self.selected_hidden_columns
+            }
+            fields.update(
+                {c.name: c.create_form_field() for c in self.can_edit_columns}
+            )
+            form_class = type(
+                "ListingRowForm{}".format(self.suffix),
+                (self.row_form_base_class,),
+                {"base_fields": fields},
+            )
             formset_class = forms.formset_factory(form_class, extra=0)
-            self._formset = formset_class(post_data, post_files,
+            self._formset = formset_class(
+                post_data,
+                post_files,
                 initial=self.get_formset_initial_values(),
-                prefix='{}{}'.format(LISTING_FORMSET_PREFIX, self.suffix)
+                prefix="{}{}".format(LISTING_FORMSET_PREFIX, self.suffix),
             )
             for form in self._formset:
                 form.listing = self
-                form.form_name = 'row_form'
+                form.form_name = "row_form"
         return self._formset
 
     def get_selected_rows(self):
         if self.request and self.request.POST:
             return self.request.POST.getlist(
-                LISTING_SELECTION_INPUT_NAME_KEY + self.suffix)
+                LISTING_SELECTION_INPUT_NAME_KEY + self.suffix
+            )
 
     def set_view(self, view):
         self._view = view
 
     def get_view(self):
         return self._view
 
 
 class DivListing(Listing):
-    listing_template_name = 'django_listing/listing_div.html'
+    listing_template_name = ThemeTemplate("listing_div.html")
+    theme_row_class = "row-container"
```

### Comparing `django-listing-0.0.9/django_listing/aggregations.py` & `django-listing-0.5.0/django_listing/aggregations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,111 +1,115 @@
 #
 # Created : 2018-24-04
 #
 # @author: Eric Lapouyade
 #
 
-from django.utils.translation import gettext_lazy as _
-from django.utils.translation import ugettext
-from django.utils.html import conditional_escape
-from django.db.models import Avg, Min, Max, Count, Sum
+from django.db.models import Avg, Max, Min, Sum
 from django.db.models.query import QuerySet
-from .html_attributes import HTMLAttributes
-from .context import RenderContext
+from django.utils.translation import gettext
+from django.utils.translation import gettext_lazy as _
+
 from .exceptions import InvalidAggregation
-from .record import Record
 
-__all__ = ['AggregationMeta','Aggregation', 'SumAggregation', 'AvgAggregation',
-           'MaxAggregation', 'MinAggregation']
+__all__ = [
+    "Aggregation",
+    "AggregationMeta",
+    "AvgAggregation",
+    "MaxAggregation",
+    "MinAggregation",
+    "SumAggregation",
+]
+
 
 class AggregationMeta(type):
     slug2class = {}
 
     def __new__(mcs, name, bases, attrs):
         cls = super(AggregationMeta, mcs).__new__(mcs, name, bases, attrs)
         AggregationMeta.slug2class[AggregationMeta.get_slug(cls)] = cls
         return cls
 
     @classmethod
     def get_slug(cls, mcs):
-        return mcs.__name__.replace('Aggregation','').lower()
+        return mcs.__name__.replace("Aggregation", "").lower()
 
     @classmethod
     def get_aggregation_slugs(cls):
-        aggs = list(filter(None,cls.slug2class.keys()))
-        return aggs + ['global_' + agg for agg in aggs ]
+        aggs = list(filter(None, cls.slug2class.keys()))
+        return aggs + ["global_" + agg for agg in aggs]
 
     @classmethod
     def get_instance(cls, slug, column):
         global_aggregation = False
-        if slug.startswith('global_'):
+        if slug.startswith("global_"):
             global_aggregation = True
             slug = slug[7:]
         agg_cls = cls.slug2class.get(slug)
         if agg_cls is None:
             raise InvalidAggregation(
-                ugettext('Unknown "{}" aggregation, choose one of these : '
-                    '{}').format(slug, ','.join(cls.get_aggregation_slugs())))
+                gettext('Unknown "{}" aggregation, choose one of these : ' "{}").format(
+                    slug, ",".join(cls.get_aggregation_slugs())
+                )
+            )
         return agg_cls(column, global_aggregation=global_aggregation)
 
 
 class Aggregation(metaclass=AggregationMeta):
     footer_tpl = None
-    value_tpl = _('{value}')
+    value_tpl = "{value}"
     params_keys = None
 
     def __init__(self, column, global_aggregation=False):
         self.values = []
         self.column = column
         self.global_aggregation = global_aggregation
         if self.params_keys:
             params_to_check = self.params_keys
-            if isinstance(params_to_check,str):
-                params_to_check = params_to_check.split(',')
+            if isinstance(params_to_check, str):
+                params_to_check = params_to_check.split(",")
             for p in params_to_check:
                 if not hasattr(column, p):
-                    setattr(column,p,getattr(self,p))
+                    setattr(column, p, getattr(self, p))
 
     def get_numeric_values(self):
-        return [ v for v in self.values if isinstance(v,(int,float)) ]
+        return [v for v in self.values if isinstance(v, (int, float))]
 
     def aggregate(self, rec):
         if not self.global_aggregation:
             value = self.column.get_cell_value(rec)
             self.values.append(value)
 
     def get_footer_attrs(self, ctx, value):
         attrs = self.column.get_footer_attrs(ctx, value)
-        attrs.add('class', 'agg-{}'.format(
-            AggregationMeta.get_slug(self.__class__)))
+        attrs.add("class", "agg-{}".format(AggregationMeta.get_slug(self.__class__)))
         return attrs
 
     def get_footer_context(self, value):
         return self.column.get_footer_context(value)
 
     def get_footer_value_tpl(self, ctx, value):
         col = self.column
-        if hasattr(col, 'get_footer_aggregation_value_tpl'):
+        if hasattr(col, "get_footer_aggregation_value_tpl"):
             return col.get_footer_aggregation_value_tpl(ctx, value)
         elif col.footer_value_tpl is not None:
             return col.footer_value_tpl
         elif self.value_tpl is not None:
             return self.value_tpl
-        return '{value}'
+        return "{value}"
 
     def get_footer_template(self, ctx, value):
         col = self.column
-        if hasattr(col, 'get_footer_aggregation_template'):
+        if hasattr(col, "get_footer_aggregation_template"):
             return col.get_footer_aggregation_template(ctx, value)
         elif col.footer_tpl is not None:
             return col.footer_tpl
         elif self.footer_tpl is not None:
             return self.footer_tpl
-        return '<td{attrs}>%s</td>' % \
-               self.get_footer_value_tpl(ctx, value)
+        return "<td{attrs}>%s</td>" % self.get_footer_value_tpl(ctx, value)
 
     def render_footer(self):
         if self.values or self.global_aggregation:
             value = self.get_aggregated_value()
             ctx = self.get_footer_context(value)
             ctx.attrs = self.get_footer_attrs(ctx, value)
             tpl = self.get_footer_template(ctx, value)
@@ -114,92 +118,101 @@
             except (ValueError, AttributeError, IndexError) as e:
                 return '<td class="render-error">{}</td>'.format(e)
         else:
             return self.column.default_footer_value
 
     def get_aggregated_value_from_sequence(self, seq):
         records = self.column.listing.records.get_all()
-        self.values = [ self.column.get_cell_value(rec) for rec in records ]
+        self.values = [self.column.get_cell_value(rec) for rec in records]
         return self.get_aggregated_value_from_current_page()
 
     def get_aggregated_value(self):
         if self.global_aggregation:
             data = self.column.listing.data
             if isinstance(data, QuerySet):
                 return self.get_aggregated_value_from_queryset(data)
             else:
                 return self.get_aggregated_value_from_sequence(data)
         else:
             return self.get_aggregated_value_from_current_page()
 
 
 class SumAggregation(Aggregation):
-    value_tpl = _('Total :<br>{value}')
+    value_tpl = _("Total :<br>{value}")
 
     def get_aggregated_value_from_current_page(self):
         return sum(self.get_numeric_values())
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(val=Sum(self.column.data_key)).get('val')
+        return qs.aggregate(val=Sum(self.column.data_key)).get("val")
 
 
 class MinAggregation(Aggregation):
-    value_tpl = _('Min :<br>{value}')
+    value_tpl = _("Min :<br>{value}")
 
     def get_aggregated_value_from_current_page(self):
         return min(self.get_numeric_values())
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(val=Min(self.column.data_key)).get('val')
+        return qs.aggregate(val=Min(self.column.data_key)).get("val")
 
 
 class MaxAggregation(Aggregation):
-    value_tpl = _('Max :<br>{value}')
+    value_tpl = _("Max :<br>{value}")
 
     def get_aggregated_value_from_current_page(self):
         return max(self.get_numeric_values())
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(val=Max(self.column.data_key)).get('val')
+        return qs.aggregate(val=Max(self.column.data_key)).get("val")
 
 
 class MinMaxAggregation(Aggregation):
-    value_tpl = _('Min : {min_val}<br>Max : {max_val}')
+    value_tpl = _("Min : {min_val}<br>Max : {max_val}")
 
     def get_aggregated_value_from_current_page(self):
-        return dict( min_val=min(self.get_numeric_values()),
-                     max_val=max(self.get_numeric_values()) )
+        return dict(
+            min_val=min(self.get_numeric_values()),
+            max_val=max(self.get_numeric_values()),
+        )
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(min_val=Min(self.column.data_key),
-                            max_val=Max(self.column.data_key))
+        return qs.aggregate(
+            min_val=Min(self.column.data_key), max_val=Max(self.column.data_key)
+        )
 
 
 class MinMaxAvgAggregation(Aggregation):
-    value_tpl = _('Min : {min_val}<br>Max : {max_val}<br>'
-                  'Avg : {avg_val:.{col.footer_precision}f}')
-    params_keys = 'footer_precision'
+    value_tpl = _(
+        "Min : {min_val}<br>Max : {max_val}<br>"
+        "Avg : {avg_val:.{col.footer_precision}f}"
+    )
+    params_keys = "footer_precision"
     footer_precision = 2
 
     def get_aggregated_value_from_current_page(self):
         num_values = self.get_numeric_values()
-        return dict( min_val=min(num_values),
-                     max_val=max(num_values),
-                     avg_val=sum(num_values)/len(num_values) )
+        return dict(
+            min_val=min(num_values),
+            max_val=max(num_values),
+            avg_val=sum(num_values) / len(num_values),
+        )
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(min_val=Min(self.column.data_key),
-                            max_val=Max(self.column.data_key),
-                            avg_val=Avg(self.column.data_key))
+        return qs.aggregate(
+            min_val=Min(self.column.data_key),
+            max_val=Max(self.column.data_key),
+            avg_val=Avg(self.column.data_key),
+        )
 
 
 class AvgAggregation(Aggregation):
-    value_tpl = 'Average :<br>{value:.{col.footer_precision}f}'
-    params_keys = 'footer_precision'
+    value_tpl = "Average :<br>{value:.{col.footer_precision}f}"
+    params_keys = "footer_precision"
     footer_precision = 2
 
     def get_aggregated_value_from_current_page(self):
         num_values = self.get_numeric_values()
-        return sum(num_values)/len(num_values)
+        return sum(num_values) / len(num_values)
 
     def get_aggregated_value_from_queryset(self, qs):
-        return qs.aggregate(val=Avg(self.column.data_key)).get('val')
+        return qs.aggregate(val=Avg(self.column.data_key)).get("val")
```

### Comparing `django-listing-0.0.9/django_listing/views.py` & `django-listing-0.5.0/django_listing/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,136 +1,152 @@
 #
 # Created : 2018-02-09
 #
 # @author: Eric Lapouyade
 #
 import json
+from urllib.parse import parse_qs
 
+from django import forms
+from django.contrib import messages
+from django.db import models
 from django.db.models import QuerySet
+from django.http import (
+    HttpResponse,
+    HttpResponseRedirect,
+    HttpResponseServerError,
+    QueryDict,
+)
+from django.template import RequestContext, loader
 from django.utils.module_loading import import_string
 from django.utils.safestring import mark_safe
-from django.views.generic import TemplateView
-from django.http import HttpResponse, HttpResponseServerError, \
-    HttpResponseRedirect, QueryDict
-from django.template import RequestContext
-from django.db import models
-from django import forms
-from django.contrib import messages
+from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
-from django.utils.translation import ugettext
-from django.template import loader
+from django.views.generic import TemplateView
+
+from .exceptions import *
 from .listing import Listing, logger
 from .listing_form import ListingForm
-from .exceptions import *
-from urllib.parse import parse_qs
-
 
 __all__ = [
-    'ListingView', 'ListingViewMixin','INSTANCE_METHOD_PREFIX',
-    'LISTING_REDIRECT_NONE', 'LISTING_REDIRECT_SAME_PAGE',
-    'LISTING_REDIRECT_NO_EDIT',
+    "INSTANCE_METHOD_PREFIX",
+    "LISTING_REDIRECT_NONE",
+    "LISTING_REDIRECT_NO_EDIT",
+    "LISTING_REDIRECT_SAME_PAGE",
+    "ListingView",
+    "ListingViewMixin",
 ]
 
-INSTANCE_METHOD_PREFIX = 'get_listing_instance_'
+from .utils import is_ajax
+
+INSTANCE_METHOD_PREFIX = "get_listing_instance_"
 LISTING_REDIRECT_NONE = None
 LISTING_REDIRECT_SAME_PAGE = 1
 LISTING_REDIRECT_NO_EDIT = 2
 
+
 class ListingViewMixin:
     listing_class = None
     listing_data = None
-    upload_field = 'image'
+    upload_field = "image"
     context_classes = ()
-    listing_context_name = 'listing'
+    listing_context_name = "listing"
     listing_instance = None
     listing = None
     insert_success_redirect_url = LISTING_REDIRECT_NONE
-    insert_success_msg = _('<b>{object}</b> has been successfully added.')
+    insert_success_msg = _("<b>{object}</b> has been successfully added.")
     insert_success_msg_no_save = _(
-        'The form is valid but nothing has been added to database '
-        'as <tt>save_to_database=False</tt>.')
+        "The form is valid but nothing has been added to database "
+        "as <tt>save_to_database=False</tt>."
+    )
     update_success_redirect_url = LISTING_REDIRECT_NONE
-    update_success_msg = _('<b>{nb_updates} {model_verbose}</b> '
-                           'has been successfully updated.')
+    update_success_msg = _(
+        "<b>{nb_updates} {model_verbose}</b> " "has been successfully updated."
+    )
     update_success_msg_no_save = _(
-        'The form is valid but nothing has been updated to database '
-        'as <tt>save_to_database=False</tt>.')
+        "The form is valid but nothing has been updated to database "
+        "as <tt>save_to_database=False</tt>."
+    )
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._listing_instances = {}
         self._formset_errors = {}
 
     def post(self, request, *args, **kwargs):
+        if hasattr(self, "get_object"):  # for DetailView that works only on GET
+            self.object = self.get_object()
         try:
-            if request.is_ajax():
-                if 'serialized_data' in request.POST:
+            if is_ajax(request):
+                if "serialized_data" in request.POST:
                     post = request.POST.copy()
-                    serialized_data = post.pop('serialized_data')
+                    serialized_data = post.pop("serialized_data")
                     if isinstance(serialized_data, list):
                         serialized_data = serialized_data[0]
                     data = parse_qs(serialized_data)
-                    for k,v in data.items():
-                        if k != 'csrfmiddlewaretoken':
+                    for k, v in data.items():
+                        if k != "csrfmiddlewaretoken":
                             if len(v) == 1:
                                 post[k] = v[0]
                             else:
                                 post[k] = v
                     request.POST = post
                 return self.manage_listing_ajax_request(request, *args, **kwargs)
             response = self.manage_listing_post(request, *args, **kwargs)
             if response:
                 return response
-            return HttpResponseRedirect('.')
+            return self.get(self, request, *args, **kwargs)
         except ListingException as e:
             return HttpResponseServerError(e)
 
     def get(self, request, *args, **kwargs):
         response = super().get(request, *args, **kwargs)
         # need to force rendering here to know whether a listing created
         # in a template has requested a data export
         response.render()
-        if hasattr(request,'export_data'):
+        if hasattr(request, "export_data"):
             data = request.export_data
-            filename = getattr(request,'export_filename','listing')
+            filename = getattr(request, "export_filename", "listing")
             response = HttpResponse(data)
-            response['Content-Disposition'] = (
-                'attachment; filename="{}"'.format(filename) )
+            response["Content-Disposition"] = 'attachment; filename="{}"'.format(
+                filename
+            )
             return response
         return response
 
     def json_response(self, data):
-        response = HttpResponse(json.dumps(data), content_type='application/json')
-        response['Cache-Control'] = 'no-cache'
+        response = HttpResponse(json.dumps(data), content_type="application/json")
+        response["Cache-Control"] = "no-cache"
         return response
 
     def get_listing_from_post(self, request, refresh=False):
-        listing_id = request.POST.get('listing_id', '')[:-3]  # remove '-id' suffix
-        listing_suffix = request.POST.get('listing_suffix', '')
+        listing_id = request.POST.get("listing_id", "")[:-3]  # remove '-id' suffix
+        listing_suffix = request.POST.get("listing_suffix", "")
         listing = self.get_listing_id(listing_id, refresh)
         if not listing:
             raise ListingException(
-                '{}-id is a bad listing ID : django-listing library misconf'
-                'iguration. Contact the webmaster !'.format(listing_id))
+                "{}-id is a bad listing ID : django-listing library misconf"
+                "iguration. Contact the webmaster !".format(listing_id)
+            )
         Listing.set_suffix(request, listing, listing_suffix)
-        listing.action = request.POST.get('force_action') or request.POST.get('action')
-        listing.action_col = request.POST.get('action_col')
+        listing.action = request.POST.get("force_action") or request.POST.get("action")
+        listing.action_col = request.POST.get("action_col")
         return listing
 
     def manage_listing_ajax_request(self, request, *args, **kwargs):
         listing = self.get_listing_from_post(request)
         self.listing = listing
         response = None
         if listing:
-            listing_part = request.POST.get('listing_part', 'all')
+            listing_part = request.POST.get("listing_part", "all")
             listing.ajax_request = True
             listing.ajax_part = listing_part
             if isinstance(listing.action, str) and listing.action:
                 listing.render_init(RequestContext(request))
-                method = getattr(self,'manage_listing_%s' % listing.action, None)
+                method = getattr(self, "manage_listing_%s" % listing.action, None)
                 if callable(method):
                     response = method(listing, *args, **kwargs)
         if response:
             return response
         if listing.have_to_refresh():
             listing = self.get_listing_from_post(request, refresh=True)
         return HttpResponse(listing.render(RequestContext(request)))
@@ -141,136 +157,145 @@
     def get_listing_data(self):
         return self.listing_data
 
     def get_listing_context_name(self):
         return self.listing_context_name
 
     def get_listing_params(self):
-        keys = ( list(Listing.get_params_keys()) +
-                 [ k for k in self.__class__.__dict__
-                   if '__' in k and not k.startswith('__') ] )  # add listing columns custimization keys (colname__attribute)
-        return { k:getattr(self,k) for k in keys if hasattr(self,k) }
+        keys = list(Listing.get_params_keys()) + [
+            k for k in self.__class__.__dict__ if "__" in k and not k.startswith("__")
+        ]  # add listing columns custimization keys (colname__attribute)
+        return {k: getattr(self, k) for k in keys if hasattr(self, k)}
 
     def get_listing_instance(self):
         data = self.get_listing_data()
         if isinstance(data, QuerySet) or data:
             listing_class = self.get_listing_class() or Listing
-            return listing_class(data,**self.get_listing_params())
+            return listing_class(data, **self.get_listing_params())
 
     # this set of methods manage a special storage because when using ajax
     # listing name are taken from div id which has been normalized
     # by replacing underscores by dashes
     def get_from_listing_instances(self, name):
-        v = self._listing_instances.get(name.replace('_','-'))
+        v = self._listing_instances.get(name.replace("_", "-"))
         if v:
             return v[1]
         return None
 
     def in_listing_instances(self, name):
-        return name.replace('_','-') in self._listing_instances
+        return name.replace("_", "-") in self._listing_instances
 
     def set_to_listing_instances(self, name, instance):
-        self._listing_instances[name.replace('_','-')] = (name, instance)
+        self._listing_instances[name.replace("_", "-")] = (name, instance)
 
     def yield_listing_instances(self):
         for v in self._listing_instances.values():
             yield v[1]
 
     def listing_instances_context(self):
         return dict(self._listing_instances.values())
 
     def get_default_listing_instance(self):
         context_name = self.get_listing_context_name()
         instance = self.get_from_listing_instances(context_name)
         if not instance:
             instance = self.get_listing_instance()
             if instance:
-                instance.id = context_name + '-id'  # Ensure id is set according to method name + '-id'
+                instance.id = (
+                    context_name + "-id"
+                )  # Ensure id is set according to method name + '-id'
                 self.set_to_listing_instances(context_name, instance)
         return instance
 
-    def get_listing_update_success_redirect_url(self, listing = None):
+    def get_listing_update_success_redirect_url(self, listing=None):
         url = self.update_success_redirect_url
         if listing:
             if url == LISTING_REDIRECT_SAME_PAGE:
                 url = listing.get_url()
             elif url == LISTING_REDIRECT_NO_EDIT:
-                url = listing.get_url(
-                    without='editing,editing_columns,editing_row_pk')
+                url = listing.get_url(without="editing,editing_columns,editing_row_pk")
         # if url = None will do a LISTING_REDIRECT_NONE : the post() will call get()
         # at the end on the same request.
         return url
 
-    def get_listing_insert_success_redirect_url(self, listing = None):
+    def get_listing_insert_success_redirect_url(self, listing=None):
         url = self.insert_success_redirect_url
         if listing:
             if url == LISTING_REDIRECT_SAME_PAGE:
                 url = listing.get_url()
-            elif url == LISTING_REDIRECT_NONE :
+            elif url == LISTING_REDIRECT_NONE:
                 # post() will call get() on-the-fly
                 # to avoid a new request to the server.
                 # That requires to reset insert form by removing Post data
                 listing.request.POST = QueryDict()
         return url
 
     def manage_listing_post(self, request, *args, **kwargs):
-        if 'action' in request.POST:
+        if "action" in request.POST:
             listing = self.get_listing_from_post(request)
             listing.set_view(self)
             self.listing = listing
             response = None
             if listing:
                 listing.render_init(RequestContext(request))
                 if isinstance(listing.action, str) and listing.action:
-                    method = getattr(self,'manage_listing_%s' % listing.action, None)
+                    method = getattr(self, "manage_listing_%s" % listing.action, None)
                     if callable(method):
                         response = method(listing, *args, **kwargs)
                 # elif listing.can_edit:
                 #     response = self.manage_listing_update(listing, *args, **kwargs)
                 # elif listing.can_select:
                 #     response = self.manage_listing_select(listing, *args, **kwargs)
             return response
 
     def manage_listing_upload(self, listing, *args, **kwargs):
         listing.model.objects.create(
-            **{self.upload_field:listing.request.FILES['file']}
+            **{self.upload_field: listing.request.FILES["file"]}
+        )
+        return self.json_response(
+            dict(
+                message="OK",
+            )
         )
-        return self.json_response(dict(message='OK',))
 
     def manage_listing_update(self, listing, *args, **kwargs):
         if listing.editable and listing.editing:
             formset = listing.get_formset()
             if formset.is_valid():
                 return self.manage_listing_update_valid(listing, formset)
             else:
                 # extract error strings from Django ErrorDict
-                listing.row_form_errors = [ ', '.join(list(e['__all__']))
-                                            for e in formset.errors
-                                            if '__all__' in e ]
+                listing.row_form_errors = [
+                    ", ".join(list(e["__all__"]))
+                    for e in formset.errors
+                    if "__all__" in e
+                ]
 
     def get_form_instance(self, listing):
         if listing.form:
             if isinstance(listing.form, ListingForm):
                 django_form = listing.form.get_form()
             elif isinstance(listing.form, forms.Form):
                 django_form = listing.form
             else:
                 if isinstance(listing.form, str):
                     form_class = import_string(listing.form)
                 else:
                     form_class = listing.form
-                django_form = form_class(listing.request.POST,
-                                         listing.request.FILES)
+                django_form = form_class(listing.request.POST, listing.request.FILES)
         else:
-            layout = listing.request.POST.get('listing_form_layout')
-            name = listing.request.POST.get('listing_form_name')
+            layout = listing.request.POST.get("listing_form_layout")
+            name = listing.request.POST.get("listing_form_name")
             if not layout or not name:
-                raise InvalidListingForm(ugettext(
-                    'At least a form layout and name are mandatory in POST data '
-                    'to build a relevant form instance'))
+                raise InvalidListingForm(
+                    gettext(
+                        "At least a form layout and name are mandatory in POST data "
+                        "to build a relevant form instance"
+                    )
+                )
             listing_form = ListingForm(listing.action, name=name, layout=layout)
             listing_form.bind_to_listing(listing)
             django_form = listing_form.get_form()
         return django_form
 
     def manage_listing_insert(self, listing, *args, **kwargs):
         form = self.get_form_instance(listing)
@@ -325,91 +350,94 @@
         self.send_listing_insert_success_message(listing, form, object)
         redirect_to = self.get_listing_insert_success_redirect_url(listing)
         if redirect_to:
             return HttpResponseRedirect(redirect_to)
 
     def send_listing_insert_success_message(self, listing, form, object):
         if listing.save_to_database:
-            msg = ( self.insert_success_msg
-                .format(listing=listing, form=form, object=object) )
+            msg = self.insert_success_msg.format(
+                listing=listing, form=form, object=object
+            )
             if msg:
-                messages.add_message(listing.request, messages.SUCCESS,
-                    mark_safe(msg))
+                messages.add_message(listing.request, messages.SUCCESS, mark_safe(msg))
         else:
-            msg = ( self.insert_success_msg_no_save
-                .format(listing=listing, form=form, object=object) )
+            msg = self.insert_success_msg_no_save.format(
+                listing=listing, form=form, object=object
+            )
             if msg:
-                messages.add_message(listing.request, messages.INFO,
-                    mark_safe(msg))
+                messages.add_message(listing.request, messages.INFO, mark_safe(msg))
 
     def send_listing_update_success_message(self, listing, updated_rows_pk):
         nb_updates = len(updated_rows_pk)
         meta = listing.model._meta
-        model_verbose = ( meta.verbose_name_plural if nb_updates > 0
-                          else meta.verbose_name_plural )
+        model_verbose = (
+            meta.verbose_name_plural if nb_updates > 0 else meta.verbose_name_plural
+        )
         if listing.save_to_database:
-            msg = ( self.update_success_msg
-                .format(listing=listing, nb_updates=nb_updates,
-                        model_verbose=model_verbose) )
+            msg = self.update_success_msg.format(
+                listing=listing, nb_updates=nb_updates, model_verbose=model_verbose
+            )
             if msg:
-                messages.add_message(listing.request, messages.SUCCESS,
-                    mark_safe(msg))
+                messages.add_message(listing.request, messages.SUCCESS, mark_safe(msg))
         else:
-            msg = ( self.update_success_msg_no_save
-                .format(listing=listing, nb_updates=nb_updates,
-                        model_verbose=model_verbose) )
+            msg = self.update_success_msg_no_save.format(
+                listing=listing, nb_updates=nb_updates, model_verbose=model_verbose
+            )
             if msg:
-                messages.add_message(listing.request, messages.INFO,
-                    mark_safe(msg))
+                messages.add_message(listing.request, messages.INFO, mark_safe(msg))
 
     def get_listing_id(self, listing_id, refresh=False):
-        """ For AJAX purposes : when using multiple listings on the same page
+        """For AJAX purposes : when using multiple listings on the same page
         and having one AJAX request : we need only ONE listing instance :
         the one from the given ID in the request. This avoids to create
-        all listing instances when not necessary """
-        if isinstance(listing_id,str):
+        all listing instances when not necessary"""
+        if isinstance(listing_id, str):
             instance = self.get_from_listing_instances(listing_id)
-            if instance is None or refresh==True:
+            if instance is None or refresh == True:
                 method = getattr(
-                    self, INSTANCE_METHOD_PREFIX + listing_id.replace('-','_'), None)
+                    self, INSTANCE_METHOD_PREFIX + listing_id.replace("-", "_"), None
+                )
                 if callable(method):
                     instance = method()
                     self.set_to_listing_instances(listing_id, instance)
                 else:
                     instance = self.get_default_listing_instance()
             if instance:
-                instance.id = listing_id + '-id'
+                instance.id = listing_id + "-id"
             return instance
         return None
 
     def get_listings_instances(self):
         prefix_length = len(INSTANCE_METHOD_PREFIX)
         # find all get_listing_instance_xxx
         for method_name in dir(self.__class__):
             if method_name.startswith(INSTANCE_METHOD_PREFIX):
-                method = getattr(self,method_name)
+                method = getattr(self, method_name)
                 if callable(method):
                     listing_id = method_name[prefix_length:]
                     if not self.in_listing_instances(listing_id):
                         instance = method()
-                        instance.id = listing_id + '-id' # Ensure id is set according to method name + '-id'
+                        instance.id = (
+                            listing_id + "-id"
+                        )  # Ensure id is set according to method name + '-id'
                         self.set_to_listing_instances(listing_id, instance)
         self.get_default_listing_instance()  # will update self._listing_instances
         for listing in self.yield_listing_instances():
             if listing.is_initialized() and not listing.is_render_initialized():
                 listing.render_init(RequestContext(self.request))
 
         return self.listing_instances_context()
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['request'] = self.request  # no need to add request context processor
-        context['posted_listing'] = self.listing
+        context["request"] = self.request  # no need to add request context processor
+        context["posted_listing"] = self.listing
         for cls in self.context_classes:
             context[cls.__name__] = cls
         if self.listing_class:
             context[self.listing_class.__name__] = self.listing_class
         context.update(self.get_listings_instances())
         return context
 
+
 class ListingView(ListingViewMixin, TemplateView):
     pass
```

### Comparing `django-listing-0.0.9/django_listing/listing_form.py` & `django-listing-0.5.0/django_listing/listing_form.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,90 @@
 #
 # Created : 2018-04-04
 #
 # @author: Eric Lapouyade
 #
 
-from django.db import models
 from django import forms
-from django.template import loader
-from django.utils.module_loading import import_string
-from django.utils.translation import gettext_lazy, pgettext_lazy
-from django.utils.translation import ugettext as _
 from django.core.exceptions import ValidationError
 from django.forms.fields import FileField
-import copy
-import re
+from django.template import loader
+from django.utils.translation import gettext as _
+from django.utils.translation import pgettext_lazy
+
 from .context import RenderContext
-from .html_attributes import HTMLAttributes
 from .exceptions import InvalidListingForm
+from .html_attributes import HTMLAttributes
+from .theme_config import ThemeTemplate
 from .utils import init_dicts_from_class
 
-
-__all__ = ['LISTING_FORM_PARAMS_KEYS', 'ListingForm']
+__all__ = ["LISTING_FORM_PARAMS_KEYS", "ListingForm"]
 
 # Declare keys only for "Filters" object
 LISTING_FORM_PARAMS_KEYS = {
-    'action', 'reset_label', 'submit_label', 'template_name',
-    'django_form_class', 'layout', 'attrs', 'buttons',
-    'ListingBaseForm',
+    "action",
+    "reset_label",
+    "submit_label",
+    "template_name",
+    "django_form_class",
+    "layout",
+    "attrs",
+    "buttons",
+    "ListingBaseForm",
 }
 
+
 class ListingBaseForm(forms.BaseForm):
     def _clean_fields(self):
         for name, field in self.fields.items():
             if field.disabled:
                 value = self.get_initial_for_field(field, name)
             else:
                 value = field.widget.value_from_datadict(
-                    self.data, self.files, self.add_prefix(name))
+                    self.data, self.files, self.add_prefix(name)
+                )
             try:
                 if isinstance(field, FileField):
                     initial = self.get_initial_for_field(field, name)
                     value = field.clean(value, initial)
                 else:
                     value = field.clean(value)
                 self.cleaned_data[name] = value
 
                 method = None
                 view = self.listing.get_view()
                 if view:
-                    method_name = f'manage_listing_{view.listing.id[:-3]}_{self.form_name}_clean_{name}'
+                    method_name = f"manage_listing_{view.listing.id[:-3]}_{self.form_name}_clean_{name}"
                     method = getattr(view, method_name, None)
                     if not method:
-                        method_name = f'manage_listing_{self.form_name}_clean_{name}'
+                        method_name = f"manage_listing_{self.form_name}_clean_{name}"
                         method = getattr(view, method_name, None)
                 if not method:
-                    method_name = f'{self.form_name}_clean_{name}'
+                    method_name = f"{self.form_name}_clean_{name}"
                     method = getattr(self.listing, method_name, None)
                 if method:
                     value = method(self)
                     self.cleaned_data[name] = value
             except ValidationError as e:
                 self.add_error(name, e)
 
     def _clean_form(self):
         try:
             method = None
             view = self.listing.get_view()
             if view:
-                method_name = f'manage_listing_{view.listing.id[:-3]}_{self.form_name}_clean'
+                method_name = (
+                    f"manage_listing_{view.listing.id[:-3]}_{self.form_name}_clean"
+                )
                 method = getattr(view, method_name, None)
                 if not method:
-                    method_name = f'manage_listing_{self.form_name}_clean'
+                    method_name = f"manage_listing_{self.form_name}_clean"
                     method = getattr(view, method_name, None)
             if not method:
-                method_name = f'{self.form_name}_clean'
+                method_name = f"{self.form_name}_clean"
                 method = getattr(self.listing, method_name, None)
             if method:
                 cleaned_data = method(self)
             else:
                 cleaned_data = self.cleaned_data
         except ValidationError as e:
             self.add_error(None, e)
@@ -87,108 +94,115 @@
 
 
 class ListingForm:
     id = None
     action = None
     form_base_class = ListingBaseForm
     django_form_class = None
-    reset_label = pgettext_lazy('Listing form', 'Reset')
-    submit_label = pgettext_lazy('Listing form', 'Add')
-    template_name = 'django_listing/listing_form.html'
+    reset_label = pgettext_lazy("Listing form", "Reset")
+    submit_label = pgettext_lazy("Listing form", "Add")
+    template_name = ThemeTemplate("listing_form.html")
     layout = None
-    buttons = 'reset,submit'
-    name = 'listing_form'
-    attrs = {'class': 'listing-form'}
+    buttons = "reset,submit"
+    name = "listing_form"
+    attrs = {"class": "listing-form"}
 
     def __init__(self, action, name=None, *args, **kwargs):
         self.init_args = args
         self.init_kwargs = kwargs
-        self.name = name or f'{action}_form'
+        self.name = name or f"{action}_form"
         self.action = action
         self._form = None
-        init_dicts_from_class(self, ['attrs',])
+        init_dicts_from_class(
+            self,
+            [
+                "attrs",
+            ],
+        )
 
     def bind_to_listing(self, listing):
         self.init(listing, *self.init_args, **self.init_kwargs)
 
     def set_listing(self, listing):
         self.listing = listing
 
-    def set_kwargs(self,**kwargs):
+    def set_kwargs(self, **kwargs):
         for k in LISTING_FORM_PARAMS_KEYS:
-            listing_key = '{}_{}'.format(self.name, k)
+            listing_key = "{}_{}".format(self.name, k)
             if k in kwargs:
                 setattr(self, k, kwargs[k])
-            elif hasattr(self.listing,listing_key):
-                setattr(self,k,getattr(self.listing,listing_key))
+            elif hasattr(self.listing, listing_key):
+                setattr(self, k, getattr(self.listing, listing_key))
 
     def init(self, listing, *args, **kwargs):
         self.set_listing(listing)
         self.set_kwargs(**kwargs)
         if isinstance(self.layout, str):
             # transform layout string into list of lists
-            self.layout = list(map(lambda s:s.split(','),
-                                        self.layout.split(';')))
+            self.layout = list(map(lambda s: s.split(","), self.layout.split(";")))
         if self.layout:
-            layout_str = ';'.join(map(lambda l:','.join(l),self.layout))
+            layout_str = ";".join(map(lambda l: ",".join(l), self.layout))
             self.listing.add_form_input_hiddens(
-                listing_form_layout=layout_str,
-                listing_form_name=self.name
+                listing_form_layout=layout_str, listing_form_name=self.name
             )
         self.listing.add_form_input_hiddens(listing_id=self.listing.id)
-        if not isinstance(self.attrs,HTMLAttributes):
+        if not isinstance(self.attrs, HTMLAttributes):
             self.attrs = HTMLAttributes(self.attrs)
-        form_css_class = 'listing-' + self.name.replace('_','-')
-        self.attrs.add('class',form_css_class)
+        form_css_class = "listing-" + self.name.replace("_", "-")
+        self.attrs.add("class", form_css_class)
         if self.listing.accept_ajax:
-            self.attrs.add('class', f'django-{self.name}-ajax')
-        if 'id' not in self.attrs:
-            self.attrs.add('id',f'{form_css_class}{self.listing.suffix}')
-        self.id = self.attrs['id']
+            self.attrs.add("class", f"django-{self.name}-ajax")
+        if "id" not in self.attrs:
+            self.attrs.add("id", f"{form_css_class}{self.listing.suffix}")
+        self.id = self.attrs["id"]
         buttons = self.buttons
-        if isinstance(buttons,str):
-            self.buttons = list(map(str.strip,buttons.split(',')))
+        if isinstance(buttons, str):
+            self.buttons = list(map(str.strip, buttons.split(",")))
 
     def datetimepicker_init(self):
-        self.listing.need_media_for('datetimepicker')
-        self.listing.add_footer_dict_list('datetimepickers', dict(
-            listing=self.listing,
-            div_id=self.id
-        ))
+        if self.listing.use_datetimepicker:
+            self.listing.need_media_for("datetimepicker")
+            self.listing.add_footer_dict_list(
+                "datetimepickers", dict(listing=self.listing, div_id=self.id)
+            )
 
     def create_form_from_layout(self):
         fields = {}
         if not self.layout:
-            raise InvalidListingForm(_('You must specify a list of columns '
-                                       'names in the form layout'))
+            raise InvalidListingForm(
+                _("You must specify a list of columns " "names in the form layout")
+            )
         for row in self.layout:
             for field_name in row:
                 col = self.listing.columns.get(field_name)
                 if not col:
                     raise InvalidListingForm(
-                        _('In the {form_name} layout you specified the field '
-                          '"{field_name}" but there is no existing listing '
-                          'column with that name')
-                        .format(form_name=self.name, field_name=field_name)
+                        _(
+                            "In the {form_name} layout you specified the field "
+                            '"{field_name}" but there is no existing listing '
+                            "column with that name"
+                        ).format(form_name=self.name, field_name=field_name)
                     )
                 fields[field_name] = col.create_form_field(have_empty_choice=True)
-        form_class = type('{}{}'.format(self.name, self.listing.suffix),
-                          (self.form_base_class,),
-                          {'base_fields': fields})
+        form_class = type(
+            "{}{}".format(self.name, self.listing.suffix),
+            (self.form_base_class,),
+            {"base_fields": fields},
+        )
         return form_class
 
     def get_form(self):
         if not self._form:
             form_class = self.create_form_from_layout()
             self._form = form_class(self.listing.request.POST or None)
             self._form.listing = self.listing
             self._form.form_name = self.name
         return self._form
 
-    def render_init(self,context):
+    def render_init(self, context):
         self.listing.manage_page_context(context)
         self.datetimepicker_init()
 
     def render(self, context):
         self.render_init(context)
         ctx = self.get_context()
         template = loader.get_template(self.template_name)
```

### Comparing `django-listing-0.0.9/django_listing/columns.py` & `django-listing-0.5.0/django_listing/columns.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,59 +13,131 @@
 
 from django import forms
 from django.conf import settings
 from django.db import models
 from django.forms import widgets
 from django.template.defaultfilters import filesizeformat
 from django.utils import formats
+from django.utils.dateparse import parse_datetime
 from django.utils.encoding import force_str
 from django.utils.html import conditional_escape
 from django.utils.safestring import mark_safe
+from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
-from django.utils.translation import ugettext
 
-from .aggregations import AggregationMeta, Aggregation
+from .aggregations import Aggregation, AggregationMeta
 from .context import RenderContext
 from .exceptions import *
 from .html_attributes import HTMLAttributes
 from .record import cache_in_record
+from .theme_config import ThemeAttribute
 from .utils import init_dicts_from_class
-from .app_settings import app_settings
 
-__all__ = ['COLUMNS_PARAMS_KEYS', 'Columns', 'ModelColumns', 'SequenceColumns',
-           'Column', 'BooleanColumn', 'CheckboxColumn', 'ChoiceColumn',
-           'ManyColumn', 'DateColumn', 'DateTimeColumn', 'TimeColumn',
-           'LinkColumn', 'TotalColumn', 'AvgColumn', 'MaxColumn', 'MinColumn',
-           'MultipleChoiceColumn','ButtonColumn','InputColumn', 'FileSizeColumn',
-           'SelectColumn', 'ForeignKeyColumn', 'LinkObjectColumn', 'ListingMethodRef',
-           'ButtonLinkColumn', 'COLUMNS_FORM_FIELD_KEYS',]
+__all__ = [
+    "AvgColumn",
+    "BooleanColumn",
+    "ButtonColumn",
+    "ButtonLinkColumn",
+    "CheckboxColumn",
+    "ChoiceColumn",
+    "Column",
+    "Columns",
+    "COLUMNS_FORM_FIELD_KEYS",
+    "COLUMNS_PARAMS_KEYS",
+    "DateColumn",
+    "DateTimeColumn",
+    "FileSizeColumn",
+    "ForeignKeyColumn",
+    "InputColumn",
+    "JsonDateTimeColumn",
+    "LinkColumn",
+    "LinkObjectColumn",
+    "ListingMethodRef",
+    "ManyColumn",
+    "MaxColumn",
+    "MinColumn",
+    "ModelColumns",
+    "MultipleChoiceColumn",
+    "SelectColumn",
+    "SequenceColumns",
+    "TimeColumn",
+    "TotalColumn",
+]
 
 COLUMNS_PARAMS_KEYS = {
-    'name', 'header', 'footer', 'data_key', 'cell_edit_tpl',
-    'cell_tpl', 'cell_attrs', 'value_tpl', 'cell_value', 'label',
-    'header_tpl', 'header_sortable_tpl',
-    'footer_tpl', 'footer_value_tpl', 'sort_key', 'sortable', 'header_attrs',
-    'footer_attrs', 'ascending_by_default', 'model_field',
-    'editable', 'default_value', 'form_field_class', 'form_field_widget_class',
-    'default_footer_value', 'aggregation', 'date_format', 'datetime_format',
-    'time_format', 'input_type', 'theme_header_class', 'theme_cell_class',
-    'theme_footer_class', 'theme_header_icon', 'widget_attrs',
-    'theme_form_widget_class','theme_button_class','no_choice_msg',
+    "aggregation",
+    "ascending_by_default",
+    "cell_attrs",
+    "cell_edit_tpl",
+    "cell_tpl",
+    "cell_value",
+    "column_class",
+    "column_instance",
+    "data_key",
+    "date_format",
+    "datetime_format",
+    "default_footer_value",
+    "default_value",
+    "editable",
+    "footer",
+    "footer_attrs",
+    "footer_tpl",
+    "footer_value_tpl",
+    "form_field_class",
+    "form_field_widget_class",
+    "header",
+    "header_attrs",
+    "header_sortable_tpl",
+    "header_tpl",
+    "input_type",
+    "label",
+    "model_field",
+    "name",
+    "no_choice_msg",
+    "sort_key",
+    "sortable",
+    "start",
+    "theme_button_class",
+    "theme_cell_class",
+    "theme_footer_class",
+    "theme_form_checkbox_widget_class",
+    "theme_form_radio_widget_class",
+    "theme_form_select_widget_class",
+    "theme_form_widget_class",
+    "theme_header_class",
+    "theme_header_icon",
+    "time_format",
+    "value_tpl",
+    "widget_attrs",
 }
 
 COLUMNS_FORM_FIELD_KEYS = {
-    'max_length','min_length','strip','empty_value','label','required',
-    'label_suffix', 'initial', 'widget', 'help_text', 'error_messages',
-    'validators', 'localize', 'disabled','input_formats','min_value',
-    'max_value',
+    "disabled",
+    "empty_value",
+    "error_messages",
+    "help_text",
+    "initial",
+    "input_formats",
+    "label",
+    "label_suffix",
+    "localize",
+    "max_length",
+    "max_value",
+    "min_length",
+    "min_value",
+    "required",
+    "strip",
+    "validators",
+    "widget",
 }
 
 
 class ListingMethodRef:
-    """ Helper to reference a Listing method in column.cell_value instead of a lambda"""
+    """Helper to reference a Listing method in column.cell_value instead of a lambda"""
+
     def __init__(self, method_name):
         self.method_name = method_name
 
     def __call__(self, listing, *args, **kwargs):
         method = getattr(listing, self.method_name)
         return method(*args, **kwargs)
 
@@ -73,214 +145,317 @@
 class Columns(list):
     def __init__(self, *cols, params=None):
         if params is None:
             params = {}
         self._params = params
         self.name2col = {}
         if cols:
-            if isinstance(cols[0],(list,tuple)):
+            if isinstance(cols[0], (list, tuple)):
                 cols = cols[0]
-            elif isinstance(cols[0],GeneratorType):
+            elif isinstance(cols[0], GeneratorType):
                 cols = list(cols[0])
         super().__init__(cols)
 
-    def get(self,name,default=None):
-        return self.name2col.get(name,default)
+    def get(self, name, default=None):
+        return self.name2col.get(name, default)
 
-    def exists(self,name):
+    def exists(self, name):
         return name in self.name2col
 
     def get_model(self):
         return None
 
     def get_params(self):
         return self._params
 
     def names(self):
-        return [ c.name for c in self ]
+        return [c.name for c in self]
 
-    def select(self,select_cols_name=None, exclude_cols_name=None):
-        if isinstance(select_cols_name,str):
-            select_cols_name = list(map(str.strip,select_cols_name.split(',')))
-        if isinstance(exclude_cols_name,str):
-            exclude_cols_name = list(map(str.strip,exclude_cols_name.split(',')))
+    def select(self, select_cols_name=None, exclude_cols_name=None):
+        if isinstance(select_cols_name, str):
+            select_cols_name = list(map(str.strip, select_cols_name.split(",")))
+        if isinstance(exclude_cols_name, str):
+            exclude_cols_name = list(map(str.strip, exclude_cols_name.split(",")))
         if select_cols_name is None:
             select_cols_name = self.names()
         exclude_cols_name = exclude_cols_name or []
-        return [ self.get(c.strip())
-                 for c in select_cols_name
-                 if c not in exclude_cols_name and c in self.name2col ]
+        cols = []
+        for col_name in select_cols_name:
+            if isinstance(col_name, (tuple, list)):
+                col_name, header = col_name
+            elif ":" in col_name:
+                col_name, header = col_name.split(":", maxsplit=1)
+            else:
+                header = None
+            col_name = col_name.replace(".", "__")
+            if col_name not in exclude_cols_name and col_name in self.name2col:
+                col = self.get(col_name.strip())
+                if col:
+                    if header:
+                        col.header = header
+                    cols.append(col)
+        return cols
 
     def bind_to_listing(self, listing):
         cols = Columns(params=self._params)
-        for i,col in enumerate(self):
+        for i, col in enumerate(self):
             # check col is a Column instance
-            if not isinstance(col,Column):
+            if not isinstance(col, Column):
                 raise InvalidColumn(
-                    ugettext('column {col_id} of listing {listing} is not '
-                             'a Column instance (class = {colclass})')
-                    .format(col_id=i, listing=listing.__class__.__name__,
-                            colclass=col.__class__.__name__))
+                    gettext(
+                        "column {col_id} of listing {listing} is not "
+                        "a Column instance (class = {colclass})"
+                    ).format(
+                        col_id=i,
+                        listing=listing.__class__.__name__,
+                        colclass=col.__class__.__name__,
+                    )
+                )
             # ensure there is one column instance per listing
             if not col.listing:
                 col = copy.deepcopy(col)
             col.bind_to_listing(listing)
             cols.append(col)
-        cols.name2col = { c.name : c for c in cols if isinstance(c,Column) }
+
+        # Auto-add foreign-key columns specified in select_columns
+        select_cols_name = listing.select_columns or []
+        if isinstance(select_cols_name, str):
+            select_cols_name = list(map(str.strip, select_cols_name.split(",")))
+        for col_name in select_cols_name:
+            if isinstance(col_name, (tuple, list)):
+                col_name = col_name[0]
+            else:
+                col_name = re.sub(":.*$", "", col_name)
+            if "." in col_name:
+                col_name = col_name.replace(".", "__")
+                data_key = col_name.replace("__", ".")
+                col = Column(col_name, data_key=data_key)
+                col.bind_to_listing(listing)
+                cols.append(col)
+
+        cols.name2col = {c.name: c for c in cols if isinstance(c, Column)}
         cols.listing = listing
         return cols
 
     def editing_init(self):
         for col in self:
             col.editing_init()
 
 
 class ModelColumns(Columns):
-    def __init__(self, model, *cols, params=None, listing=None,
-                 link_object_columns=None, **kwargs):
-        if params is None:
-            params = {}
-        if not link_object_columns:
-            link_object_columns = ''
-        if isinstance(link_object_columns, str):
-            link_object_columns = set(map(str.strip,link_object_columns.split(',')))
+    def __init__(
+        self,
+        model,
+        *cols,
+        params=None,
+        listing=None,
+        link_object_columns=None,
+        **kwargs,
+    ):
+        self.model = model
+        self.cols = cols
+        self.params = params
+        self.listing = listing
+        self.link_object_columns = link_object_columns
+        self.kwargs = kwargs
+
+    def set_listing(self, listing):
+        self.listing = listing
+
+    def init(self):
+        if self.params is None:
+            self.params = {}
+        if not self.link_object_columns:
+            self.link_object_columns = ""
+        if isinstance(self.link_object_columns, str):
+            self.link_object_columns = set(
+                map(str.strip, self.link_object_columns.split(","))
+            )
 
         model_cols = []
         # when not yet initialized, column name is in init_args[0]
-        name2col = OrderedDict( (c.name or c.init_args[0],c) for c in cols )
-        for f in model._meta.get_fields():
-            if not isinstance(f, (models.ManyToManyRel,models.ManyToOneRel)):
-                header = getattr(f,'verbose_name',f.name)
+        name2col = OrderedDict((c.name or c.init_args[0], c) for c in self.cols)
+        select_columns = []
+        if self.listing:
+            if isinstance(self.listing.select_columns, str):
+                select_columns = list(
+                    map(str.strip, self.listing.select_columns.split(","))
+                )
+            else:
+                select_columns = self.listing.select_columns or []
+
+        for f in self.model._meta.get_fields():
+            if f.name in select_columns or not isinstance(
+                f, (models.ManyToManyRel, models.ManyToOneRel)
+            ):
+                if not hasattr(self.listing, f"{f.name}__header"):
+                    header = getattr(f, "verbose_name", f.name.capitalize())
+                else:
+                    header = getattr(self.listing, f"{f.name}__header")
+                col_class = getattr(self.listing, f"{f.name}__column_class", None)
+                if col_class and not issubclass(col_class, Column):
+                    raise InvalidColumn(
+                        f"{f.name}__override_class must be a class derived from "
+                        f"Column class"
+                    )
+                col_instance = getattr(self.listing, f"{f.name}__column_instance", None)
+                if col_instance and not isinstance(col_instance, Column):
+                    raise InvalidColumn(
+                        f"{f.name}__override_instance must be an instance of Column "
+                        f"class or a derived class"
+                    )
                 if f.name in name2col:
                     col = name2col.pop(f.name)
+                    col.header = header
                     model_cols.append(col)
                 else:
-                    if f.name in link_object_columns:
-                        model_cols.append(LinkObjectColumn(
-                            f.name, model_field=f,
-                            header=header,**kwargs)
+                    if col_instance:
+                        col_instance.header = header
+                        col_instance.model_field = f
+                        model_cols.append(col_instance)
+                    elif col_class:
+                        model_cols.append(
+                            col_class(
+                                f.name, model_field=f, header=header, **self.kwargs
+                            )
+                        )
+                    elif f.name in self.link_object_columns:
+                        model_cols.append(
+                            LinkObjectColumn(
+                                f.name, model_field=f, header=header, **self.kwargs
+                            )
                         )
                     else:
-                        model_cols.append(self.create_column(
-                            f,header=header,
-                            **kwargs)
+                        model_cols.append(
+                            self.create_column(f, header=header, **self.kwargs)
                         )
 
         super().__init__(*(model_cols + list(name2col.values())))
-        if listing:
+        if self.listing:
             for col in self:
-                col.set_listing(listing)
-        self._model = model
-        self._params = params
+                col.set_listing(self.listing)
+        self._model = self.model
+        self._params = self.params
 
     @classmethod
     def create_column_name(cls, listing, name, **kwargs):
         model = listing.model
         if model:
             model_field = model._meta.get_field(name)
             if not model_field:
                 return None
-            header = getattr(model_field, 'verbose_name', model_field.name)
+            if not hasattr(listing, f"{model_field.name}__header"):
+                header = getattr(model_field, "verbose_name", model_field.name)
+            else:
+                header = getattr(listing, f"{model_field.name}__header")
             col = cls.create_column(model_field, header=header, **kwargs)
             col.bind_to_listing(listing)
             return col
 
     def get_model(self):
         return self._model
 
     @classmethod
     def create_column(cls, field, **kwargs):
         field_name = field.name
         for col_class in ColumnMeta.get_column_classes():
             if col_class is not Column:
-                col = col_class.from_model_field(field,**kwargs)
+                col = col_class.from_model_field(field, **kwargs)
                 if col:
                     return col
         return Column(field_name, model_field=field, **kwargs)
 
 
 class SequenceColumns(Columns):
-    def __init__(self, seq, columns_headers=None, params=None,
-                 listing=None, **kwargs):
-        if params is None:
-            params = {}
-        first_row = seq[0]
+    def __init__(self, seq, columns_headers=None, params=None, listing=None, **kwargs):
+        self.seq = seq
+        self.columns_headers = columns_headers
+        self.params = params
+        self.listing = listing
+        self.kwargs = kwargs
+
+    def set_listing(self, listing):
+        self.listing = listing
+
+    def init(self):
+        if self.params is None:
+            self.params = {}
+        first_row = self.seq[0]
         if not isinstance(first_row, (dict, list, tuple)):
-            for i,v in enumerate(seq):
-                seq[i] = [seq[i]]
-            first_row = seq[0]
+            for i, v in enumerate(self.seq):
+                self.seq[i] = [self.seq[i]]
+            first_row = self.seq[0]
         cols = []
         if isinstance(first_row, dict):
-            if not isinstance(columns_headers,dict):
-                columns_headers={}
-            for k,v in first_row.items():
-                header = columns_headers.get(k)
-                cols.append(self.create_column(v, k, header=header, **kwargs))
+            if not isinstance(self.columns_headers, dict):
+                self.columns_headers = {}
+            for k, v in first_row.items():
+                header = self.columns_headers.get(k)
+                cols.append(self.create_column(v, k, header=header, **self.kwargs))
         elif isinstance(first_row, (list, tuple)):
-            if not isinstance(columns_headers,(list, tuple)):
-                columns_headers=()
-            for i,v in enumerate(first_row):
-                if i < len(columns_headers) and columns_headers[i]:
-                    header = columns_headers[i]
+            if not isinstance(self.columns_headers, (list, tuple)):
+                self.columns_headers = ()
+            for i, v in enumerate(first_row):
+                if i < len(self.columns_headers) and self.columns_headers[i]:
+                    header = self.columns_headers[i]
                 else:
-                    header = 'Column{}'.format(i + 1)
-                cols.append(self.create_column(v, header=header,
-                                               data_key=i, **kwargs))
+                    header = "Column{}".format(i + 1)
+                cols.append(
+                    self.create_column(v, header=header, data_key=i, **self.kwargs)
+                )
         super().__init__(*cols)
-        if listing:
+        if self.listing:
             for col in self:
-                col.set_listing(listing)
-        self._params = params
+                col.set_listing(self.listing)
+        self._params = self.params
 
     @classmethod
-    def create_column(cls, value, name=None,
-                      header=None, data_key=None, **kwargs):
-        if isinstance(value,datetime.datetime):
-            return DateTimeColumn(name, header=header,
-                                  data_key=data_key, **kwargs)
-        elif isinstance(value,datetime.date):
-            return DateColumn(name, header=header,data_key=data_key, **kwargs)
-        return Column(name, header=header,data_key=data_key, **kwargs)
+    def create_column(cls, value, name=None, header=None, data_key=None, **kwargs):
+        if isinstance(value, datetime.datetime):
+            return DateTimeColumn(name, header=header, data_key=data_key, **kwargs)
+        elif isinstance(value, datetime.date):
+            return DateColumn(name, header=header, data_key=data_key, **kwargs)
+        return Column(name, header=header, data_key=data_key, **kwargs)
 
 
 class ColumnMeta(type):
     column_classes = []
 
     def __new__(mcs, name, bases, attrs):
         cls = super(ColumnMeta, mcs).__new__(mcs, name, bases, attrs)
-        ColumnMeta.column_classes.append((cls,cls.from_model_field_order))
+        ColumnMeta.column_classes.append((cls, cls.from_model_field_order))
         params_keys = cls.params_keys
-        if isinstance(params_keys,str):
-            params_keys = set(map(str.strip,params_keys.split(',')))
+        if isinstance(params_keys, str):
+            params_keys = set(map(str.strip, params_keys.split(",")))
         COLUMNS_PARAMS_KEYS.update(params_keys)
-        COLUMNS_PARAMS_KEYS.discard('')
+        COLUMNS_PARAMS_KEYS.discard("")
         form_field_keys = cls.form_field_keys
         if form_field_keys:
-            if isinstance(form_field_keys,str):
-                form_field_keys = set(map(str.strip,form_field_keys.split(',')))
+            if isinstance(form_field_keys, str):
+                form_field_keys = set(map(str.strip, form_field_keys.split(",")))
             COLUMNS_FORM_FIELD_KEYS.update(form_field_keys)
-            COLUMNS_FORM_FIELD_KEYS.discard('')
+            COLUMNS_FORM_FIELD_KEYS.discard("")
             COLUMNS_PARAMS_KEYS.update(COLUMNS_FORM_FIELD_KEYS)
         return cls
 
     @classmethod
     def get_column_classes(cls):
-        return [ t[0] for t in sorted(cls.column_classes,key=lambda x:x[1]) ]
+        return [t[0] for t in sorted(cls.column_classes, key=lambda x: x[1])]
 
 
 class Column(metaclass=ColumnMeta):
     aggregation = None
     ascending_by_default = True
     can_edit = False
     cell_tpl = None
     cell_edit_tpl = None
     cell_value = None
     data_key = None
-    default_footer_value = ''
-    default_value = '-'
+    default_footer_value = ""
+    default_value = "-"
     editable = None
     editing = False
     footer = None
     footer_tpl = None
     footer_value_tpl = None
     form_field_class = forms.CharField
     form_field_widget_class = None
@@ -291,125 +466,169 @@
     header_sortable_tpl = None
     header_tpl = None
     help_text = None
     input_type = None
     listing = None
     model_field = None
     name = None
-    no_choice_msg = _('Please choose...')
-    params_keys = ''
+    no_choice_msg = _("Please choose...")
+    params_keys = ""
     sort_key = None
     sortable = True
-    value_tpl = '{value}'
+    value_tpl = "{value}"
 
-    theme_header_class = ''
-    theme_cell_class = ''
-    theme_footer_class = ''
-    theme_form_widget_class = 'form-control form-control-sm'
-    theme_button_class = 'btn btn-primary btn-sm'
+    theme_header_class = ThemeAttribute("column_theme_header_class")
+    theme_cell_class = ThemeAttribute("column_theme_cell_class")
+    theme_footer_class = ThemeAttribute("column_theme_footer_class")
+    theme_form_widget_class = ThemeAttribute("column_theme_form_widget_class")
+    theme_form_select_widget_class = ThemeAttribute(
+        "column_theme_form_select_widget_class"
+    )
+    theme_form_checkbox_widget_class = ThemeAttribute(
+        "column_theme_form_checkbox_widget_class"
+    )
+    theme_form_radio_widget_class = ThemeAttribute(
+        "column_theme_form_radio_widget_class"
+    )
+    theme_button_class = ThemeAttribute("column_theme_button_class")
 
     def __init__(self, *args, **kwargs):
         self.init_args = args
         self.init_kwargs = kwargs
-        init_dicts_from_class(self, ['cell_attrs', 'header_attrs', 'cell_attrs',
-                                     'footer_attrs', 'widget_attrs'])
+        init_dicts_from_class(
+            self,
+            [
+                "cell_attrs",
+                "header_attrs",
+                "cell_attrs",
+                "footer_attrs",
+                "widget_attrs",
+            ],
+        )
 
     def bind_to_listing(self, listing):
         self.init(listing, *self.init_args, **self.init_kwargs)
 
     def set_listing(self, listing):
         self.listing = listing
 
     def init(self, listing, name=None, **kwargs):
         self.set_listing(listing)
-        header = kwargs.get('header')
+        header = kwargs.get("header")
         if name:
-            self.name = re.sub(r'\W','',name)
+            self.name = re.sub(r"\W", "", name)
         if self.name is None:
             if header:
-                self.name = re.sub(r'\W', '',header.strip().replace(' ','_').lower())
+                self.name = re.sub(r"\W", "", header.strip().replace(" ", "_").lower())
             else:
-                self.name = 'noname'
+                self.name = "noname"
         self.set_kwargs(**kwargs)
         self.apply_template_kwargs()
         if self.data_key is None:
             self.data_key = self.name
         if self.sort_key is None:
-            self.sort_key = self.data_key
-        if isinstance(self.aggregation,str):
-            self.aggregation = AggregationMeta.get_instance(self.aggregation,self)
-        if isinstance(self.theme_header_class,str):
+            if isinstance(self.data_key, str):
+                self.sort_key = self.data_key.replace(".", "__")
+            else:
+                self.sort_key = 0
+        if isinstance(self.aggregation, str):
+            self.aggregation = AggregationMeta.get_instance(self.aggregation, self)
+        if isinstance(self.theme_header_class, str):
             self.theme_header_class = set(self.theme_header_class.split())
-        if isinstance(self.theme_cell_class,str):
+        if isinstance(self.theme_cell_class, str):
             self.theme_cell_class = set(self.theme_cell_class.split())
-        if isinstance(self.theme_footer_class,str):
+        if isinstance(self.theme_footer_class, str):
             self.theme_footer_class = set(self.theme_footer_class.split())
-        if isinstance(self.theme_form_widget_class,str):
+        if isinstance(self.theme_form_widget_class, str):
             self.theme_form_widget_class = set(self.theme_form_widget_class.split())
-        if isinstance(self.theme_button_class,str):
+        if isinstance(self.theme_form_select_widget_class, str):
+            self.theme_form_select_widget_class = set(
+                self.theme_form_select_widget_class.split()
+            )
+        if isinstance(self.theme_form_checkbox_widget_class, str):
+            self.theme_form_checkbox_widget_class = set(
+                self.theme_form_checkbox_widget_class.split()
+            )
+        if isinstance(self.theme_form_radio_widget_class, str):
+            self.theme_form_radio_widget_class = set(
+                self.theme_form_radio_widget_class.split()
+            )
+        if isinstance(self.theme_button_class, str):
             self.theme_button_class = set(self.theme_button_class.split())
 
     def render_init(self):
         pass
 
     def editing_init(self):
         # editable attribute can be set via 'editable_columns'
         # only if not already set in the final column class
-        if self.editable is None and {'all',self.name} & self.listing.editable_columns:
+        if self.editable is None and {"all", self.name} & self.listing.editable_columns:
             self.editable = True
-        if {'all',self.name} & self.listing.editing_columns:
+        if {"all", self.name} & self.listing.editing_columns:
             self.editing = True
-        self.can_edit = ( self.editable and self.editing and
-                          self.listing.editable and self.listing.editing )
+        self.can_edit = (
+            self.editable
+            and self.editing
+            and self.listing.editable
+            and self.listing.editing
+        )
 
     def set_kwargs(self, **kwargs):
         # if parameters given in columns : apply them
-        for k, v in self.listing.columns.get_params().get(self.name,{}).items():
+        for k, v in self.listing.columns.get_params().get(self.name, {}).items():
             if k in COLUMNS_PARAMS_KEYS:
                 setattr(self, k, v)
         for k in COLUMNS_PARAMS_KEYS | COLUMNS_FORM_FIELD_KEYS:
-            listing_key = 'columns_{}'.format(k)
-            if hasattr(self.listing,listing_key):
-                setattr(self,k,getattr(self.listing,listing_key))
+            listing_key = "columns_{}".format(k)
+            if hasattr(self.listing, listing_key):
+                setattr(self, k, getattr(self.listing, listing_key))
         # col__param has higher priority than columns_param,
-        # so getting col__params after columns_params
-        for k, v in self.listing.__class__.__dict__.items():
-            start_key = f'{self.name}__'
-            if k.startswith(start_key):
-                setattr(self, k[len(start_key):], v)
+        # so getting col__params AFTER columns_params
         for k, v in kwargs.items():
             if k in COLUMNS_PARAMS_KEYS:
-                setattr(self,k,v)
+                setattr(self, k, v)
+        # DO NOT swap with above for-loop, otherwise <col>__choices won't work
+        # See showcase BoolChoicesImgColumnsListing "gender" column
+        for k in dir(self.listing):
+            start_key = f"{self.name}__"
+            if k.startswith(start_key):
+                v = getattr(self.listing, k)
+                setattr(self, k[len(start_key) :], v)
 
     def apply_template_kwargs(self):
         kwargs = self.listing.get_column_kwargs(self.name)
         if kwargs:
             for k, v in kwargs.items():
                 if k in COLUMNS_PARAMS_KEYS:
-                    if isinstance(v,dict):
-                        prev_value = getattr(self,k,None)
-                        if isinstance(prev_value,dict):
+                    if isinstance(v, dict):
+                        prev_value = getattr(self, k, None)
+                        if isinstance(prev_value, dict):
                             prev_value.update(v)
                             continue
-                    setattr(self,k,v)
+                    setattr(self, k, v)
 
     @classmethod
     def from_model_field(cls, field, **kwargs):
         if field.__class__ in cls.from_model_field_classes:
             return cls(field.name, model_field=field, **kwargs)
 
     def get_cell_attrs(self, rec, ctx, value):
         cell_attrs = self.cell_attrs
         if callable(cell_attrs):
             cell_attrs = cell_attrs(rec, ctx, value)
         attrs = HTMLAttributes(cell_attrs)
-        attrs.add('class', {'col-'+self.name,
-                           'type-'+type(value).__name__,
-                           'cls-'+self.__class__.__name__.lower()
-                           } | self.theme_cell_class)
+        attrs.add(
+            "class",
+            {
+                "col-" + self.name,
+                "type-" + type(value).__name__,
+                "cls-" + self.__class__.__name__.lower(),
+            }
+            | self.theme_cell_class,
+        )
         return attrs
 
     def get_default_value(self, rec):
         return self.default_value
 
     # def get_raw_value(self, rec):
     #     return rec.get(self.data_key)
@@ -420,49 +639,60 @@
             value = self.cell_value(self.listing, self, rec)
         elif callable(self.cell_value):
             value = self.cell_value(self, rec)
         else:
             value = rec.get(self.data_key)
             if value is None:
                 value = self.get_default_value(rec)
+        if hasattr(self, "choices"):
+            value = self.choices.get(value, value)
+        return value
+
+    def get_cell_form_value(self, rec):
+        value = rec.get(self.data_key)
         return value
 
-    def get_cell_exported_value(self,rec):
+    def get_cell_exported_value(self, rec):
         val = self.get_cell_value(rec)
-        if not isinstance(val,(int, float, datetime.datetime,
-                               datetime.date,datetime.time)):
+        if not isinstance(
+            val, (int, float, datetime.datetime, datetime.date, datetime.time)
+        ):
             return force_str(val)
         return val
 
     def render_form_field(self, rec):
         """Render a cell edit field when a listing is being edited"""
 
         # get the django form field (a formset form is attached to each record)
         # you get an instance of forms.CharField, forms.DateField etc...
         form_field = rec.get_form()[self.name]
         errors = form_field.errors
         if errors:
-            html = ('<div class="form-field errors"><span class='
-                     '"listing-icon-attention"></span>{errors}{form_field}</div>').format(
-                     errors=errors, form_field=form_field)
+            html = (
+                '<div class="form-field errors"><span class='
+                '"listing-icon-attention"></span>{errors}{form_field}</div>'
+            ).format(errors=errors, form_field=form_field)
         else:
             html = ('<div class="form-field">{form_field}</div>').format(
-                    form_field=form_field)
+                form_field=form_field
+            )
         return html
 
     def get_cell_context(self, rec, value):
-        if isinstance(value,str):
+        if isinstance(value, str):
             value = conditional_escape(value)
-        return RenderContext(self.listing.global_context,
-                             rec.get_format_ctx(),
-                             value,  # if value is a dict it will be merged (see RenderContext)
-                             value=value,  # if value is not a dict it will have the key 'value' in the context
-                             rec=rec,
-                             listing=self.listing,
-                             col=self)
+        return RenderContext(
+            self.listing.global_context,
+            rec.get_format_ctx(),
+            value,  # if value is a dict it will be merged (see RenderContext)
+            value=value,  # if value is not a dict it will have the key 'value' in the context
+            rec=rec,
+            listing=self.listing,
+            col=self,
+        )
 
     def get_edit_value_tpl(self, rec, ctx, value):
         return self.render_form_field(rec)
 
     def get_value_tpl(self, rec, ctx, value):
         value_tpl = self.value_tpl
         if callable(value_tpl):
@@ -472,180 +702,207 @@
     def get_cell_template(self, rec, ctx, value):
         if self.can_edit and rec.get_form() is not None:
             value_tpl = self.get_edit_value_tpl(rec, ctx, value)
             cell_tpl = self.cell_edit_tpl or self.cell_tpl
         else:
             cell_tpl = self.cell_tpl
             value_tpl = self.get_value_tpl(rec, ctx, value)
-        tpl = cell_tpl or '<td{attrs}>%s</td>'
+        tpl = cell_tpl or "<td{attrs}>%s</td>"
         return tpl % value_tpl
 
-    def render_cell(self,rec):
+    def render_cell(self, rec):
         value = self.get_cell_value(rec)
         ctx = self.get_cell_context(rec, value)
         ctx.attrs = self.get_cell_attrs(rec, ctx, value)
         tpl = self.get_cell_template(rec, ctx, value)
         try:
             return tpl.format(**ctx)
         except (ValueError, AttributeError, IndexError) as e:
             return '<td class="render-error">{}</td>'.format(e)
 
     def get_header_attrs(self, ctx):
         header_attrs = self.header_attrs
         if callable(header_attrs):
             header_attrs = header_attrs(ctx)
         attrs = HTMLAttributes(header_attrs)
-        if self.sortable:
-            attrs.add('class',self.listing.theme_sortable_class)
+        if self.sortable and self.listing.sortable:
+            attrs.add("class", self.listing.theme_sortable_class)
             asc = self.listing.columns_sort_ascending.get(self.name)
             if asc is not None:
-                attrs.add('class', self.listing.theme_sort_asc_class if asc else
-                                   self.listing.theme_sort_desc_class)
-        attrs.add('class', {'col-'+self.name} | self.theme_header_class)
+                attrs.add("class", self.listing.theme_sorted_class)
+                attrs.add(
+                    "class",
+                    self.listing.theme_sort_asc_class
+                    if asc
+                    else self.listing.theme_sort_desc_class,
+                )
+        else:
+            attrs.add("class", "not-sortable")
+        attrs.add("class", {"col-" + self.name} | self.theme_header_class)
         return attrs
 
     def get_header_value(self):
         if self.header:
             if callable(self.header):
                 # call to lambda function with column and listing as arguments
-                header_value = self.header(self,self.listing)
+                header_value = self.header(self, self.listing)
             else:
                 header_value = self.header
         else:
-            header_value = self.name.replace('_', ' ').title()
+            header_value = self.name.replace("_", " ").title()
         return header_value
 
     def get_header_context(self):
         sort_url = None
         icon = None
         if self.sortable and self.listing.sortable:
             actual_ascending = self.listing.columns_sort_ascending.get(self.name)
-            ascending = not self.ascending_by_default \
-                        if actual_ascending is None \
-                        else actual_ascending
-            sort_param = '{}{}'.format('-' if ascending else '',self.name)
-            if ( actual_ascending is not None
-                 and actual_ascending != self.ascending_by_default
-                 and self.listing.unsortable ):
-                sort_url = self.listing.get_url(without='sort')
+            ascending = (
+                not self.ascending_by_default
+                if actual_ascending is None
+                else actual_ascending
+            )
+            sort_param = "{}{}".format("-" if ascending else "", self.name)
+            if (
+                actual_ascending is not None
+                and actual_ascending != self.ascending_by_default
+                and self.listing.unsortable
+            ):
+                sort_url = self.listing.get_url(without="sort")
             else:
                 sort_url = self.listing.get_url(sort=sort_param)
             asc = self.listing.columns_sort_ascending.get(self.name)
             if asc is None:
                 icon = self.listing.theme_sort_none_icon
             elif asc:
                 icon = self.listing.theme_sort_asc_icon
             else:
                 icon = self.listing.theme_sort_desc_icon
             if icon:
-                icon = ' ' + icon
+                icon = " " + icon
         value = self.get_header_value()
         if isinstance(value, str):
             value = conditional_escape(value)
         return RenderContext(
             self.listing.global_context,
             value,  # if value is a dict it will be merged (see RenderContext)
             value=value,  # if value is not a dict it will have the key 'value' in the context
             sort_url=sort_url,
             icon=icon,
             listing=self.listing,
-            col=self)
+            col=self,
+        )
 
     def get_header_template(self, ctx):
         if ctx.sort_url:
             return self.header_sortable_tpl or (
-                   '<th{attrs}><a class="listing-nav" href="{sort_url}">{value}'
-                   '<span class="sorting{icon}"></span></a></th>')
+                '<th{attrs}><a class="listing-nav" href="{sort_url}">{value}'
+                '<span class="sorting{icon}"></span></a></th>'
+            )
         else:
-            return self.header_tpl or '<th{attrs}>{value}</th>'
+            return self.header_tpl or "<th{attrs}>{value}</th>"
 
     def render_header(self):
         ctx = self.get_header_context()
         ctx.attrs = self.get_header_attrs(ctx)
         tpl = self.get_header_template(ctx)
         return tpl.format(**ctx)
 
     def get_footer_attrs(self, ctx, value):
         footer_attrs = self.footer_attrs
         if callable(footer_attrs):
             footer_attrs = footer_attrs(ctx)
         attrs = HTMLAttributes(footer_attrs)
-        attrs.add('class',{'col-'+self.name,
-                           'type-'+type(value).__name__,
-                           'cls-'+self.__class__.__name__.lower()
-                           } | self.theme_footer_class )
+        attrs.add(
+            "class",
+            {
+                "col-" + self.name,
+                "type-" + type(value).__name__,
+                "cls-" + self.__class__.__name__.lower(),
+            }
+            | self.theme_footer_class,
+        )
         return attrs
 
     def get_footer_value(self):
         if callable(self.footer):
             # call to lambda function with column and listing as arguments
-            footer_value = self.footer(self,self.listing)
+            footer_value = self.footer(self, self.listing)
         else:
             footer_value = self.footer
         if footer_value is None:
             return self.default_footer_value
         return footer_value
 
     def get_footer_context(self, value):
         if isinstance(value, str):
             value = conditional_escape(value)
         return RenderContext(
             self.listing.global_context,
             value,  # if value is a dict it will be merged (see RenderContext)
             value=value,  # if value is not a dict it will have the key 'value' in the context
             listing=self.listing,
-            col=self)
+            col=self,
+        )
 
     def get_footer_value_tpl(self, ctx, value):
-        footer_value_tpl = self.footer_value_tpl or '{value}'
+        footer_value_tpl = self.footer_value_tpl or "{value}"
         if callable(footer_value_tpl):
             footer_value_tpl = footer_value_tpl(ctx, value)
         return footer_value_tpl
 
     def get_footer_template(self, ctx, value):
-        return self.footer_tpl or '<td{attrs}>%s</td>' % \
-                    self.get_footer_value_tpl(ctx, value)
+        return self.footer_tpl or "<td{attrs}>%s</td>" % self.get_footer_value_tpl(
+            ctx, value
+        )
 
     def render_footer(self):
         if isinstance(self.aggregation, Aggregation):
             return self.aggregation.render_footer()
         value = self.get_footer_value()
         ctx = self.get_footer_context(value)
         ctx.attrs = self.get_footer_attrs(ctx, value)
         tpl = self.get_footer_template(ctx, value)
         try:
             return tpl.format(**ctx)
         except (ValueError, AttributeError, IndexError) as e:
             return '<td class="render-error">{}</td>'.format(e)
 
     def get_form_field_params(self, have_empty_choice=False):
-        params = { p:getattr(self,p) for p in COLUMNS_FORM_FIELD_KEYS
-                   if getattr(self,p,None) is not None }
+        params = {
+            p: getattr(self, p)
+            for p in COLUMNS_FORM_FIELD_KEYS
+            if getattr(self, p, None) is not None
+        }
         return params
 
     def get_form_field_class(self):
         cls = self.form_field_class
         if isinstance(cls, str):
             cls = getattr(forms, cls, None)
             if cls is None:
                 raise InvalidColumn(
-                    ugettext('{} is not a valid django forms field class')
-                    .format(self.form_field_class))
+                    gettext("{} is not a valid django forms field class").format(
+                        self.form_field_class
+                    )
+                )
         return cls
 
     def get_form_field_widget(self, field_class):
         cls = self.form_field_widget_class or field_class.widget
         if isinstance(cls, str):
             cls = getattr(widgets, cls, None)
             if cls is None:
                 raise InvalidColumn(
-                    ugettext('{} is not a valid django forms widget class')
-                    .format(self.form_field_widget_class))
-        widget_attrs=HTMLAttributes(self.widget_attrs)
-        widget_attrs.add('class',self.theme_form_widget_class)
+                    gettext("{} is not a valid django forms widget class").format(
+                        self.form_field_widget_class
+                    )
+                )
+        widget_attrs = HTMLAttributes(self.widget_attrs)
+        widget_attrs.add("class", self.theme_form_widget_class)
         return cls(attrs=widget_attrs)
 
     def create_form_field(self, have_empty_choice=False):
         cls = self.get_form_field_class()
         params = self.get_form_field_params(have_empty_choice)
         widget = self.get_form_field_widget(cls)
         field = cls(widget=widget, **params)
@@ -657,279 +914,324 @@
     def create_hidden_form_field(self):
         cls = self.get_form_field_class()
         params = self.get_hidden_form_field_params()
         widget = widgets.HiddenInput()
         field = cls(widget=widget, **params)
         return field
 
-    def set_params_choices(self,params):
-        if not params.get('choices'):
-            if getattr(self,'model_field',None):
-                params['choices'] = self.model_field.choices
+    def set_params_choices(self, params):
+        if not params.get("choices"):
+            if getattr(self, "model_field", None):
+                params["choices"] = self.model_field.choices
             elif self.listing.model:
                 try:
                     model = self.listing.model
-                    params['choices'] = model._meta.get_field(self.name).choices
+                    params["choices"] = model._meta.get_field(self.name).choices
                 except (models.FieldDoesNotExist, AttributeError):
-                    raise InvalidFilters(_('Cannot find choices from model '
-                        'for filter "{name}", Please specify the choices to '
-                        'display').format(name=self.name))
+                    raise InvalidFilters(
+                        _(
+                            "Cannot find choices from model "
+                            'for filter "{name}", Please specify the choices to '
+                            "display"
+                        ).format(name=self.name)
+                    )
             else:
-                raise InvalidFilters(_('Please specify the choices to display '
-                    'for filter "{name}"').format(name = self.name ))
+                raise InvalidFilters(
+                    _(
+                        "Please specify the choices to display " 'for filter "{name}"'
+                    ).format(name=self.name)
+                )
+
 
 class TextColumn(Column):
     from_model_field_classes = (models.TextField,)
     form_field_widget_class = widgets.Textarea
-    widget_attrs = {'rows':'3'}
+    widget_attrs = {"rows": "3"}
 
 
 class BooleanColumn(Column):
-    true_tpl = _('True')
-    false_tpl = _('False')
-    params_keys = 'true_tpl,false_tpl'
+    true_tpl = _("True")
+    false_tpl = _("False")
+    params_keys = "true_tpl,false_tpl"
     from_model_field_classes = (models.BooleanField, models.NullBooleanField)
     form_field_class = forms.BooleanField
     required = False
 
     def get_value_tpl(self, rec, ctx, value):
         return self.true_tpl if value else self.false_tpl
 
+    def get_form_field_widget(self, field_class):
+        wiget_attrs = HTMLAttributes(self.widget_attrs)
+        wiget_attrs.add("class", "form-check-input")
+        return forms.CheckboxInput(attrs=wiget_attrs)
+
 
 class IntegerColumn(Column):
     from_model_field_classes = (models.IntegerField,)
     form_field_class = forms.IntegerField
 
 
 class ChoiceColumn(Column):
-    choices={}
-    params_keys = 'choices'
+    choices = {}
+    params_keys = "choices"
     from_model_field_order = 50
     form_field_class = forms.ChoiceField
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
-        if not isinstance(self.choices,dict):
+        if not isinstance(self.choices, dict):
             self.choices = OrderedDict(self.choices)
 
     @classmethod
     def from_model_field(cls, field, **kwargs):
-        if hasattr(field, 'choices') and field.choices:
-            return ChoiceColumn(field.name,
-                                model_field=field,
-                                choices=OrderedDict(field.choices),
-                                **kwargs)
+        if hasattr(field, "choices") and field.choices:
+            return ChoiceColumn(
+                field.name,
+                model_field=field,
+                choices=OrderedDict(field.choices),
+                **kwargs,
+            )
 
-    def get_value_tpl(self,rec, ctx, value):
-        return self.choices.get(value,value)
+    def get_value_tpl(self, rec, ctx, value):
+        return self.choices.get(value, value)
 
     def get_form_field_params(self, have_empty_choice=False):
         params = super().get_form_field_params()
         self.set_params_choices(params)
-        if have_empty_choice and self.input_type not in ('radio','radioinline'):
-            params['choices'] = [ ('', self.no_choice_msg) ] + \
-                                list(params['choices'])
+        if have_empty_choice and self.input_type not in ("radio", "radioinline"):
+            params["choices"] = [("", self.no_choice_msg)] + list(params["choices"])
         return params
 
     def get_form_field_widget(self, field_class):
-        if self.input_type == 'radio':
-            return forms.RadioSelect(
-                attrs={'class':'multiple-radios'})
-        elif self.input_type == 'radioinline':
-            return forms.RadioSelect(
-                attrs={'class':'multiple-radios inline'})
-        return super().get_form_field_widget(field_class)
+        widget_attrs = HTMLAttributes(self.widget_attrs)
+        if self.input_type == "radio":
+            widget = forms.RadioSelect
+            widget_attrs.add("class", self.theme_form_radio_widget_class)
+            widget_attrs.add("class", "multiple-radios")
+        elif self.input_type == "radioinline":
+            widget = forms.RadioSelect
+            widget_attrs.add("class", self.theme_form_radio_widget_class)
+            widget_attrs.add("class", "multiple-radios inline")
+        else:
+            widget = forms.Select
+            widget_attrs.add("class", self.theme_form_select_widget_class)
+        return widget(attrs=widget_attrs)
 
 
 class MultipleChoiceColumn(Column):
-    choices={}
-    params_keys = 'choices'
+    choices = {}
+    params_keys = "choices"
     from_model_field_order = 90
     form_field_class = forms.MultipleChoiceField
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
-        if not isinstance(self.choices,dict):
+        if not isinstance(self.choices, dict):
             self.choices = OrderedDict(self.choices)
 
     @classmethod
     def from_model_field(cls, field, **kwargs):
-        if hasattr(field, 'choices') and field.choices:
-            return MultipleChoiceColumn(field.name,
-                                model_field=field,
-                                choices=OrderedDict(field.choices),
-                                **kwargs)
+        if hasattr(field, "choices") and field.choices:
+            return MultipleChoiceColumn(
+                field.name,
+                model_field=field,
+                choices=OrderedDict(field.choices),
+                **kwargs,
+            )
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
-        return self.choices.get(value,value)
+        return self.choices.get(value, value)
 
     def get_form_field_params(self, have_empty_choice=False):
         params = super().get_form_field_params()
         self.set_params_choices(params)
-        if have_empty_choice and self.input_type not in ('checkbox','checkboxinline'):
-            params['choices'] = [ ('', self.no_choice_msg) ] + \
-                                list(params['choices'])
+        if have_empty_choice and self.input_type not in ("checkbox", "checkboxinline"):
+            params["choices"] = [("", self.no_choice_msg)] + list(params["choices"])
         return params
 
     def get_form_field_widget(self, field_class):
-        if self.input_type == 'checkbox':
-            return forms.CheckboxSelectMultiple(
-                attrs={'class':'multiple-checkboxes'})
-        elif self.input_type == 'checkboxinline':
-            return forms.CheckboxSelectMultiple(
-                attrs={'class':'multiple-checkboxes inline'})
-        return super().get_form_field_widget(field_class)
+        widget_attrs = HTMLAttributes(self.widget_attrs)
+        if self.input_type == "checkbox":
+            widget = forms.CheckboxSelectMultiple
+            widget_attrs.add("class", self.theme_form_radio_widget_class)
+            widget_attrs.add("class", "multiple-checkboxes")
+        elif self.input_type == "checkboxinline":
+            widget = forms.CheckboxSelectMultiple
+            widget_attrs.add("class", self.theme_form_radio_widget_class)
+            widget_attrs.add("class", "multiple-checkboxes inline")
+        else:
+            widget = forms.CheckboxInput
+            widget_attrs.add("class", self.theme_form_select_widget_class)
+        return widget(attrs=widget_attrs)
 
 
 class ManyColumn(Column):
-    many_separator = ', '
-    params_keys = 'many_separator,cell_map,cell_filter,cell_reduce'
-    from_model_field_classes = (models.ManyToManyField,)
+    many_separator = ", "
+    params_keys = "many_separator,cell_map,cell_filter,cell_reduce"
+    from_model_field_classes = (models.ManyToManyField, models.ManyToManyRel)
     editable = False
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         value = self.cell_filter(value)
-        value = map(self.cell_map,value)
+        value = map(self.cell_map, value)
         value = self.cell_reduce(value)
         return value
 
-    def cell_filter(self,value):
-        if isinstance(value,models.Manager):
+    def cell_filter(self, value):
+        if isinstance(value, models.Manager):
             value = value.all()
         return value
 
-    def cell_map(self,value):
+    def cell_map(self, value):
         return force_str(value)
 
-    def cell_reduce(self,value):
+    def cell_reduce(self, value):
         return self.many_separator.join(value)
 
 
 class CheckboxColumn(Column):
     sortable = False
 
-    def get_value_tpl(self,rec, ctx, value):
+    def get_value_tpl(self, rec, ctx, value):
         attrs = HTMLAttributes(self.widget_attrs)
-        attrs.add('type','checkbox')
-        attrs.add('name',self.name)
+        attrs.add("type", "checkbox")
+        attrs.add("name", self.name)
+        attrs.add("class", self.theme_form_checkbox_widget_class)
         # If a value is set at definition time : take it
         # otherwise : take cell value
         if self.cell_value is not None:
             value = self.cell_value
         if value:
-            attrs.set('checked')
-        return '<input{}>'.format(attrs)
+            attrs.set("checked")
+        return "<input{}>".format(attrs)
 
 
 class ButtonColumn(Column):
-    label = 'Button'
+    label = "Button"
     sortable = False
 
-    def get_value_tpl(self,rec, ctx, value):
+    def get_value_tpl(self, rec, ctx, value):
         attrs = HTMLAttributes(self.widget_attrs)
-        attrs.add('type','button')
-        attrs.add('name',self.name)
-        attrs.add('class',self.theme_button_class)
-        return '<button{attrs}>{label}</button>'.format(
-            attrs=attrs,label=conditional_escape(self.label))
+        attrs.add("type", "button")
+        attrs.add("name", self.name)
+        attrs.add("class", self.theme_button_class)
+        return "<button{attrs}>{label}</button>".format(
+            attrs=attrs, label=conditional_escape(self.label)
+        )
 
 
 class SelectColumn(Column):
     sortable = False
-    choices={}
+    choices = {}
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
-        if not isinstance(self.choices,dict):
+        if not isinstance(self.choices, dict):
             self.choices = OrderedDict(self.choices)
 
-    def get_value_tpl(self,rec, ctx, value):
+    def get_value_tpl(self, rec, ctx, value):
         attrs = HTMLAttributes(self.widget_attrs)
-        attrs.add('name',self.name)
-        attrs.add('class',self.theme_form_widget_class)
+        attrs.add("name", self.name)
+        attrs.add("class", self.theme_form_select_widget_class)
         # If a value is set at definition time : take it
         # otherwise : take cell value
         if self.cell_value is not None:
             value = self.cell_value
-        options = [ '<option value="{key}"{sel}>{val}</option>\n'
-            .format( key=k,
-                     val=conditional_escape(v),
-                     sel=' selected' if value==k else '')
-            for k,v in self.choices.items() ]
-        return '<select{}>\n{}</select>'.format(attrs, options)
+        options = [
+            '<option value="{key}"{sel}>{val}</option>\n'.format(
+                key=k, val=conditional_escape(v), sel=" selected" if value == k else ""
+            )
+            for k, v in self.choices.items()
+        ]
+        return "<select{}>\n{}</select>".format(attrs, options)
 
 
 class InputColumn(Column):
-    widget_attrs = {'type':'text'}
+    widget_attrs = {"type": "text"}
     sortable = False
 
-    def get_value_tpl(self,rec, ctx, value):
+    def get_value_tpl(self, rec, ctx, value):
         attrs = HTMLAttributes(self.widget_attrs)
-        attrs.add('name',self.name)
-        attrs.add('class',self.theme_form_widget_class)
-        return '<input{attrs}>'.format(attrs=attrs)
+        attrs.add("name", self.name)
+        attrs.add("class", self.theme_form_widget_class)
+        return "<input{attrs}>".format(attrs=attrs)
 
 
 class DateColumn(Column):
     date_format = settings.DATE_FORMAT
-    params_keys = 'date_format'
+    params_keys = "date_format"
     from_model_field_classes = (models.DateField,)
     form_field_class = forms.DateField
-    widget_attrs = {'class': 'edit-datecolumn', 'autocomplete':'off'}
+    widget_attrs = {"class": "edit-datecolumn", "autocomplete": "off"}
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):
             return formats.date_format(value, self.date_format)
         return value
 
 
 class DateTimeColumn(Column):
     datetime_format = settings.DATETIME_FORMAT
-    params_keys = 'datetime_format'
+    params_keys = "datetime_format"
     from_model_field_classes = (models.DateTimeField,)
-    widget_attrs = {'class': 'edit-datetimecolumn', 'autocomplete':'off'}
+    widget_attrs = {"class": "edit-datetimecolumn", "autocomplete": "off"}
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):  # date also match datetime
             return formats.date_format(value, self.datetime_format)
         return value
 
 
+class JsonDateTimeColumn(Column):
+    datetime_format = settings.DATETIME_FORMAT
+    params_keys = "datetime_format"
+
+    def get_cell_value(self, rec):
+        value = super().get_cell_value(rec)
+        if isinstance(value, str):
+            value = (
+                parse_datetime(value) or value
+            )  # convert json date to datetime object
+        if isinstance(value, datetime.date):  # date also match datetime
+            return formats.date_format(value, self.datetime_format)
+        return value
+
+
 class FileSizeColumn(Column):
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         if isinstance(value, (int, float)):
             return filesizeformat(value)
         return value
 
 
 class TimeColumn(Column):
     time_format = settings.TIME_FORMAT
-    params_keys = 'time_format'
+    params_keys = "time_format"
     from_model_field_classes = (models.TimeField,)
-    widget_attrs = {'class': 'edit-timecolumn', 'autocomplete':'off'}
+    widget_attrs = {"class": "edit-timecolumn", "autocomplete": "off"}
 
     def get_cell_value(self, rec):
         value = super().get_cell_value(rec)
         if isinstance(value, datetime.date):  # date also match datetime
             return formats.time_format(value, self.time_format)
         return value
 
 
 class LinkColumn(Column):
-    params_keys = 'link_attrs,href_tpl,no_link'
+    params_keys = "link_attrs,href_tpl,no_link"
     href_tpl = None
     no_link = False
     link_attrs = None
-    cell_tpl = '<td{attrs}><a{link_attrs}>%s</a></td>'
-    cell_edit_tpl = '<td{attrs}>%s</td>'
+    cell_tpl = "<td{attrs}><a{link_attrs}>%s</a></td>"
+    cell_edit_tpl = "<td{attrs}>%s</td>"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_link_attrs(self, rec, value):
         link_attrs = self.link_attrs
         if isinstance(link_attrs, ListingMethodRef):
@@ -943,71 +1245,71 @@
         href_tpl = self.href_tpl
         if isinstance(href_tpl, ListingMethodRef):
             href_tpl = href_tpl(self.listing, self, rec, value)
         elif callable(href_tpl):
             href_tpl = href_tpl(rec, value)
         return href_tpl
 
-    def get_href(self,rec, ctx, value):
+    def get_href(self, rec, ctx, value):
         href_tpl = self.get_href_tpl(rec, value)
         if isinstance(href_tpl, str):
             return href_tpl.format(**ctx)
         return None
 
     def get_cell_context(self, rec, value):
         ctx = super().get_cell_context(rec, value)
         ctx.link_attrs = self.get_link_attrs(rec, value)
         if not self.no_link:
-            ctx.link_attrs.add('href', self.get_href(rec, ctx, value))
+            ctx.link_attrs.add("href", self.get_href(rec, ctx, value))
         return ctx
 
 
 class ButtonLinkColumn(LinkColumn):
-    label = 'Button'
+    label = "Button"
 
     def get_link_attrs(self, rec, value):
         attrs = super().get_link_attrs(rec, value)
-        attrs.add('class', self.theme_button_class)
+        attrs.add("class", self.theme_button_class)
         return attrs
 
     def get_cell_value(self, rec):
         value = mark_safe(self.label)
         return value
 
 
 class URLColumn(LinkColumn):
-    href_tpl = '{value}'
+    href_tpl = "{value}"
     from_model_field_classes = (models.URLField,)
     form_field_widget_class = widgets.URLInput
-    params_keys = 'remove_proto'
+    params_keys = "remove_proto"
     remove_proto = True
 
     def get_cell_context(self, rec, value):
         ctx = super().get_cell_context(rec, value)
         if self.remove_proto and not self.can_edit:
-            ctx.value = re.sub('^.*?//','',ctx.value)
+            ctx.value = re.sub("^.*?//", "", ctx.value)
         return ctx
 
 
 class EmailColumn(LinkColumn):
-    href_tpl = 'mailto:{value}'
+    href_tpl = "mailto:{value}"
     from_model_field_classes = (models.EmailField,)
     form_field_widget_class = widgets.EmailInput
 
 
 class LinkObjectColumn(LinkColumn):
     editable = False
 
     def get_href(self, rec, ctx, value):
         return rec.get_href()
 
 
 class ForeignKeyColumn(LinkColumn):
     from_model_field_classes = (models.ForeignKey,)
-    params_keys = 'no_foreignkey_link'
+    params_keys = "no_foreignkey_link"
     no_foreignkey_link = False
     editable = False
 
     def get_href(self, rec, ctx, value):
         if self.no_foreignkey_link:
             return None
         if self.href_tpl:
@@ -1017,117 +1319,140 @@
         except (IndexError, AttributeError):
             return super().get_href(rec, ctx, value)
 
 
 class FileColumn(LinkColumn):
     from_model_field_classes = (models.FileField,)
     form_field_class = forms.FileField
-    params_keys = 'check_file, path_tpl, no_file_link'
+    params_keys = "check_file, path_tpl, no_file_link"
     check_file = True
     no_file_link = False
-    path_tpl = '{MEDIA_ROOT}/{value.name}'
+    path_tpl = "{MEDIA_ROOT}/{value.name}"
 
     def get_path_tpl(self, rec, ctx, value):
         path_tpl = self.path_tpl
         if callable(path_tpl):
             path_tpl = path_tpl(rec, ctx, value)
         return path_tpl
 
     def get_href(self, rec, ctx, value):
         if self.no_file_link:
             return None
         url = None
         if self.check_file:
-            storage = getattr(value, 'storage', None)
+            storage = getattr(value, "storage", None)
             if storage:
                 if storage.exists(value.name):
                     if self.href_tpl:
                         url = super().get_href(rec, ctx, value)
                     else:
                         url = storage.url(value.name)
             else:
                 path = self.get_path_tpl(rec, ctx, value).format(**ctx)
                 if os.path.exists(path):
                     url = super().get_href(rec, ctx, value)
             if not url:
-                ctx.link_attrs.add('class', 'missing')
+                ctx.link_attrs.add("class", "missing")
         return url
 
 
 class ComputedColumnMixin:
     editable = False
     sortable = False
 
-    def get_row_numeric_values(self,rec):
+    def get_row_numeric_values(self, rec):
         values = []
         for col in self.listing.selected_columns:
             if not isinstance(col, ComputedColumnMixin):
                 value = col.get_cell_value(rec)
                 if isinstance(value, (int, float)):
                     values.append(value)
         return values
 
 
 class TotalColumn(ComputedColumnMixin, Column):
-    name = 'cc_total'  # 'cc' for computed column
-    header = _('Total')
-    aggregation = 'sum'  # aggregate rows
-    footer_tpl = _('<td{attrs}>Grand Total:<br>{value}</td>')
+    name = "cc_total"  # 'cc' for computed column
+    header = _("Total")
+    aggregation = "sum"  # aggregate rows
+    footer_tpl = _("<td{attrs}>Grand Total:<br>{value}</td>")
 
     @cache_in_record
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         return sum(self.get_row_numeric_values(rec))  # aggregate columns
 
 
 class MinColumn(ComputedColumnMixin, Column):
-    name = 'cc_min_value'
-    header = _('Min')
-    aggregation = 'min'
-    footer_tpl = _('<td{attrs}>Overall Min:<br>{value}</td>')
+    name = "cc_min_value"
+    header = _("Min")
+    aggregation = "min"
+    footer_tpl = _("<td{attrs}>Overall Min:<br>{value}</td>")
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         return min(self.get_row_numeric_values(rec))
 
 
 class MaxColumn(ComputedColumnMixin, Column):
-    name = 'cc_max_value'
-    header = _('Max')
-    aggregation = 'max'
-    footer_tpl = _('<td{attrs}>Overall Max:<br>{value}</td>')
+    name = "cc_max_value"
+    header = _("Max")
+    aggregation = "max"
+    footer_tpl = _("<td{attrs}>Overall Max:<br>{value}</td>")
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         return max(self.get_row_numeric_values(rec))
 
 
 class AvgColumn(ComputedColumnMixin, Column):
-    params_keys = 'precision, footer_precision'
-    name = 'cc_average'
-    header = _('Average')
+    params_keys = "precision, footer_precision"
+    name = "cc_average"
+    header = _("Average")
     precision = 2
     footer_precision = 2
-    value_tpl = '{value:.{col.precision}f}'
-    aggregation = 'avg'
-    footer_tpl = _('<td{attrs}>Overall avg:<br>{value:.{col.footer_precision}f}</td>')
+    value_tpl = "{value:.{col.precision}f}"
+    aggregation = "avg"
+    footer_tpl = _("<td{attrs}>Overall avg:<br>{value:.{col.footer_precision}f}</td>")
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         values = self.get_row_numeric_values(rec)
         if values:
-            return sum(values)/len(values)
+            return sum(values) / len(values)
         return self.default_value
 
 
+class LineNumberColumn(Column):
+    name = "auto_line_number"
+    header = "#"
+    sortable = False
+    start = 1
+
+    def get_cell_value(self, rec):
+        current_page = getattr(rec.get_listing(), "current_page", None)
+        page_start = current_page.start_index() if current_page else 1
+        return page_start + rec.get_index() + self.start - 1
+
+
 class SelectionColumn(Column):
     sortable = False
-    theme_header_icon = 'listing-icon-ok'
-    header_tpl = '<th{attrs}><span class={col.theme_header_icon}></span></th>'
+    theme_header_icon = "listing-icon-ok"
+    header_tpl = "<th{attrs}><span class={col.theme_header_icon}></span></th>"
 
     def get_cell_context(self, rec, value):
         context = super().get_cell_context(rec, value)
-        context['selection_value'] = rec.get(self.listing.selection_key)
-        context['checked'] = ' checked' if rec.is_selected() else ''
+        context["selection_value"] = rec.get(self.listing.selection_key)
+        context["checked"] = " checked" if rec.is_selected() else ""
         return context
 
     def get_value_tpl(self, rec, ctx, value):
         if self.listing.selection_multiple:
-            return '<input type="checkbox" name="selected_rows{listing.suffix}" class="selection-box" value="{selection_value}"{checked}>'
+            widget_class = " ".join(self.theme_form_checkbox_widget_class)
+            tpl = (
+                '<input type="checkbox" name="selected_rows{listing.suffix}" '
+                f'class="selection-box {widget_class}" '
+                'value="{selection_value}"{checked}>'
+            )
         else:
-            return '<input type="radio" name="selected_rows{listing.suffix}" class="selection-box" value="{selection_value}"{checked}>'
+            widget_class = " ".join(self.theme_form_radio_widget_class)
+            tpl = (
+                '<input type="radio" name="selected_rows{listing.suffix}" '
+                f'class="selection-box {widget_class}" '
+                'value="{selection_value}"{checked}>'
+            )
+        return tpl
```

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/js/django_listing.js` & `django-listing-0.5.0/django_listing/static/django_listing/js/django_listing.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -54,14 +54,15 @@
         function(responseText, textStatus, req) {
             if (textStatus == "error") {
                 listing_div.removeClass("spinning");
                 alert(responseText);
             } else {
                 $(this).children(":first").unwrap();
             }
+            $(document).trigger("djlst_ajax_loaded", [listing_target]);
         } // to avoid cascade of listing container divs
     );
     return false;
 }
 
 function djlst_load_listing_href() {
     return djlst_load_listing_url($(this), $(this).attr("href"));
@@ -119,19 +120,26 @@
         row.find('input.selection-box').first().prop('checked', true);
     }
     djlst_selection_menu_update($(this));
 }
 
 function djlst_unique_row_select(e) {
     var row = $(this).closest('.row-container');
-    row.siblings().removeClass('selected').find('input.row-select').removeAttr('name');
     var hidden = row.find('input.row-select').first();
-    row.addClass('selected');
-    hidden.attr('name', hidden.attr('select-name'));
-    row.find('input.selection-box').first().prop('checked', true);
+    if (row.hasClass('selected')) {
+        row.removeClass('selected');
+        hidden.removeAttr('name');
+        row.find('input.selection-box').first().prop('checked', false);
+    } else {
+        row.siblings().removeClass('selected').find('input.row-select').removeAttr('name');
+        row.addClass('selected');
+        hidden.attr('name', hidden.attr('select-name'));
+        row.find('input.selection-box').first().prop('checked', true);
+    }
+    djlst_selection_menu_update($(this));
 }
 
 
 function djlst_select_all(e) {
     var listing_id = $(this).attr('listing-target');
     var listing = $('#' + listing_id);
     listing.find('.row-container').addClass('selected');
@@ -200,23 +208,25 @@
             break;
     }
 }
 
 function djlst_selection_menu_update(e) {
     var listing = e.closest("div.django-listing-selecting");
     var selection_menu_id = listing.attr('selection-menu-id');
-    var selection_menu = $('#' + selection_menu_id);
-    var selected_items = selection_menu.find('span.selected_items')
-    var count = listing.find('.row-container.selected').length;
-    if (count == 0) {
-        selected_items.text(selected_items.attr('none'));
-    } else if (count == 1) {
-        selected_items.text(selected_items.attr('one'));
-    } else {
-        selected_items.text(selected_items.attr('many').replace('{nb}', count));
+    if (selection_menu_id) {
+        var selection_menu = $('#' + selection_menu_id);
+        var selected_items = selection_menu.find('span.selected_items')
+        var count = listing.find('.row-container.selected').length;
+        if (count == 0) {
+            selected_items.text(selected_items.attr('none'));
+        } else if (count == 1) {
+            selected_items.text(selected_items.attr('one'));
+        } else {
+            selected_items.text(selected_items.attr('many').replace('{nb}', count));
+        }
     }
 }
 
 function djlst_view_object_popup(event) {
     event.preventDefault();
     var nav_obj = $(this);
     var listing_div = nav_obj.closest("div.django-listing-container");
@@ -241,14 +251,16 @@
             $("#listing-popup-container > div.modal").modal("show");
         }
     });
 }
 
 $(document).ready(function() {
 
+    var select2_opened = false;
+
     $('form.listing-form').submit(function() {
         $(this).find('input[name]').filter(function() {
             return !this.value;
         }).prop('name', '');
     });
 
     $(document.body).on("click", "div.django-listing-ajax button.listing-nav", djlst_post_button_action);
@@ -286,8 +298,28 @@
     $('.submit-action-form').on('click', function() {
         var action = $(this).val();
         var form = $(this).closest('.django-listing-container').find('.action-form');
         var hidden = form.find('.action-hidden-value');
         hidden.val(action);
         form.submit();
     });
+
+    $(document).on('select2:open', () => {
+        document.querySelector('.select2-search__field').focus();
+        select2_opened = true;
+    });
+
+    $("form").keyup(function(e) {
+        if (e.keyCode == 9) {
+            const target = $(e.target)
+            if (target.hasClass("select2-selection")) {
+                if (!select2_opened) {
+                    target.closest(".select2").siblings("select").first().select2("open");
+                }
+                select2_opened = true;
+            } else {
+                select2_opened = false;
+            }
+        }
+    });
+
 });
```

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/csv.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/csv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/json.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/json.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/xlsx.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/pdf.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/dbf.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/dbf.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/xls.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/xls.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/tsv.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/tsv.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/html.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/html.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/icons/ods.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/icons/ods.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-embedded.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-embedded.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-codes.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7-codes.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7-codes.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing-ie7.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing-ie7.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/django_listing.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/django_listing.css`

 * *Files 4% similar despite different names*

```diff
@@ -386,145 +386,147 @@
     -moz-transform: rotate(359deg);
     -o-transform: rotate(359deg);
     -webkit-transform: rotate(359deg);
     transform: rotate(359deg);
   }
 }
 
-div.django-listing-container.standard-theme table.django-listing th {
+div.django-listing-container table.django-listing th {
     vertical-align: text-bottom;
 }
 
-div.django-listing-container.standard-theme table.django-listing th.sortable a {
+div.django-listing-container table.django-listing th.sortable a {
     padding-right: 20px;
     display: block;
     position: relative;
     text-decoration: none;
 }
 
-div.django-listing-container.standard-theme table.django-listing th.sortable span.sorting {
+div.django-listing-container table.django-listing th.sortable span.sorting {
     position: absolute;
     top: 0px;
     right: 0px;
     bottom: 0px;
     width: 20px;
 }
 
-div.django-listing-container.standard-theme table.django-listing {
+div.django-listing-container table.django-listing {
     margin: 0 0 6px 0;
     width: 100%;
 }
 
-div.django-listing-container.standard-theme table.django-listing.table-bordered {
+div.django-listing-container table.django-listing.table-bordered {
     box-shadow: 0 1px 3px rgba(0, 0, 0, 0.2);
     display: table;
 }
 
-div.django-listing-container.standard-theme div.django-listing div.div-row {
+div.django-listing-container div.django-listing div.div-row {
     display: -webkit-box;
     display: -ms-flexbox;
     display: flex;
     -ms-flex-wrap: wrap;
     flex-wrap: wrap;
 }
 
-div.django-listing-container.standard-theme div.django-listing.div-striped div.row-container:nth-of-type(odd) {
+div.django-listing-container div.django-listing.div-striped div.row-container:nth-of-type(odd) {
     background: #e9e9e9;
 }
 
-div.django-listing-container.standard-theme div.django-listing.div-hover div.row-container:hover {
+div.django-listing-container div.django-listing.div-hover div.row-container:hover {
     background: #ccc;
 }
 
-div.django-listing-container.standard-theme div.django-listing.div-bordered {
+div.django-listing-container div.django-listing.div-bordered {
     border: 1px solid #cccccc;
 }
 
-div.django-listing-container.standard-theme ul.pagination {
+div.django-listing-container ul.pagination {
     justify-content: center;
     align-items: center;
 }
 
-div.django-listing-container.standard-theme ul.pagination-groups {
+div.django-listing-container ul.pagination-groups {
     margin-top: 20px;
     display: flex;
     justify-content: center;
     align-items: center;
     padding-left: 0;
 }
 
-div.django-listing-container.standard-theme ul.pagination-groups > li {
+div.django-listing-container ul.pagination-groups > li {
     list-style: none;
     margin: 0;
     padding: 0;
 }
 
-div.django-listing-container.standard-theme div.variationstoolbaritem ul {
+div.django-listing-container div.variationstoolbaritem ul {
     display: flex;
     justify-content: center;
     align-items: center;
     margin: 0;
     padding: 0;
 }
 
-div.django-listing-container.standard-theme div.variationstoolbaritem li {
+div.django-listing-container div.variationstoolbaritem li {
     list-style: none;
 }
 
-div.django-listing-container.standard-theme nav.toolbar label {
+div.django-listing-container nav.toolbar label {
     margin: 0;
 }
 
-div.django-listing-container.standard-theme ul.pagination li.scale_pages ul {
+div.django-listing-container ul.pagination li.scale_pages ul {
     padding: 0 10px;
     list-style: none;
     display: flex;
 }
 
-div.django-listing-container.standard-theme ul li.pagination-info {
+div.django-listing-container ul li.pagination-info {
     padding: 0 10px;
 }
 
-div.django-listing-container.standard-theme ul li.row-info {
+div.django-listing-container ul li.row-info {
     padding: 0 10px;
 }
 
-div.django-listing-container.standard-theme ul li.goto-page {
+div.django-listing-container ul li.goto-page {
     padding: 0 10px;
 }
 
-div.django-listing-container.standard-theme .btn-toolbar select {
+div.django-listing-container .btn-toolbar select {
     font-family: django_listing, arial;
     height: 24px;
     vertical-align: middle;
 }
 
-div.django-listing-container.standard-theme .btn-toolbar .sortdropdowntoolbaritem a {
+div.django-listing-container .btn-toolbar .sortdropdowntoolbaritem a {
     font-family: django_listing, arial;
 }
 
-div.django-listing-container.standard-theme form.goto-page {
+div.django-listing-container form.goto-page {
     display:inline;
 }
 
-div.django-listing-container.standard-theme form.goto-page input {
+div.django-listing-container form.goto-page input {
     width: 40px;
 }
 
 
-div.django-listing-container.standard-theme td.cls-totalcolumn {
+div.django-listing-container td.cls-totalcolumn {
     font-weight: bold;
 }
 
-div.django-listing-container td.type-str.cls-filesizecolumn,
-div.django-listing-container td.type-int,
-div.django-listing-container td.type-float,
-div.django-listing-container td.agg-minmax,
-div.django-listing-container td.agg-minmaxavg {
-    text-align: right;
+@media (min-width: 768px) {
+    div.django-listing-container td.type-str.cls-filesizecolumn,
+    div.django-listing-container td.type-int,
+    div.django-listing-container td.type-float,
+    div.django-listing-container td.agg-minmax,
+    div.django-listing-container td.agg-minmaxavg {
+        text-align: right;
+    }
 }
 
 div.django-listing-container td.type-bool  {
     vertical-align: middle;
 }
 
 div.django-listing-container td.type-bool input {
@@ -678,15 +680,15 @@
     cursor: pointer;
 }
 
 div.django-listing-selecting.selection_position_hidden tr {
     cursor: pointer;
 }
 
-div.django-listing-container.standard-theme thead th.col-selection_checkbox  {
+div.django-listing-container thead th.col-selection_checkbox  {
     vertical-align: middle;
 }
 
 div.django-listing-container div.row-container {
     position: relative;
 }
```

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/css/animation.css` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/css/animation.css`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.eot` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.eot`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.svg` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.svg`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.woff`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.ttf` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.ttf`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/static/django_listing/font/django_listing.woff2` & `django-listing-0.5.0/django_listing/static/django_listing/bootstrap4/font/django_listing.woff2`

 * *Files identical despite different names*

### Comparing `django-listing-0.0.9/django_listing/exceptions.py` & `django-listing-0.5.0/django_listing/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 #
 
 
 class ListingException(Exception):
     pass
 
 
+class InvalidListingConfiguration(ListingException):
+    pass
+
+
 class InvalidListing(ListingException):
     pass
 
 
 class InvalidColumn(ListingException):
     pass
```

### Comparing `django-listing-0.0.9/django_listing/toolbar.py` & `django-listing-0.5.0/django_listing/toolbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 #
 # Created : 2018-02-09
 #
 # @author: Eric Lapouyade
 #
+import copy
+import re
+from itertools import count
+from types import GeneratorType
 
-from .html_attributes import HTMLAttributes
 from django.utils.translation import gettext_lazy as _
-from types import GeneratorType
-import copy
+
+from django_listing import EXPORT_FORMATS
+
 from .context import RenderContext
 from .exceptions import *
-from .utils import normalize_list, normalize_choices
-from django_listing import EXPORT_FORMATS
-from itertools import count
-import re
+from .html_attributes import HTMLAttributes
+from .theme_config import ThemeAttribute, ThemeTemplate
+from .utils import normalize_choices, normalize_list
 
 __all__ = [
-    'TOOLBAR_PARAMS_KEYS', 'Toolbar', 'ToolbarItem',
-    'SortSelectToolbarItem', 'VariationsToolbarItem',
-    'PerPageSelectToolbarItem', 'ExportSelectToolbarItem',
-    'PerPageDropdownToolbarItem', 'ExportDropdownToolbarItem',
-    'SortDropdownToolbarItem', 'UpdateToolbarItem',
+    "ExportDropdownToolbarItem",
+    "ExportSelectToolbarItem",
+    "PerPageDropdownToolbarItem",
+    "PerPageSelectToolbarItem",
+    "SortDropdownToolbarItem",
+    "SortSelectToolbarItem",
+    "TOOLBAR_PARAMS_KEYS",
+    "Toolbar",
+    "ToolbarItem",
+    "UpdateToolbarItem",
+    "VariationsToolbarItem",
 ]
 
 TOOLBAR_PARAMS_KEYS = {
-    'name', 'label', 'button_label','template_name', 'attrs', 'choices',
-    'theme_button_class',
+    "attrs",
+    "button_label",
+    "choices",
+    "label",
+    "name",
+    "template_name",
+    "theme_button_class",
 }
 
+
 class Toolbar(list):
-    template_name = 'django_listing/toolbar.html'
+    template_name = ThemeTemplate("toolbar.html")
 
     def __init__(self, *items, params=None, listing=None):
         if params is None:
             params = {}
         self._params = params
         self.name2item = {}
         if items:
             if isinstance(items[0], str):
-                items_name = map(str.strip, items[0].split(','))
+                items_name = map(str.strip, items[0].split(","))
                 items = []
                 for name in items_name:
-                    slug = re.sub('[_\d]+$','',name)
+                    slug = re.sub("[_\d]+$", "", name)
                     cls = ToolbarItemMeta.get_class(slug)
                     item = cls(name)
                     item.set_listing(listing)
                     items.append(cls(name))
-            elif isinstance(items[0],(list,tuple)):
+            elif isinstance(items[0], (list, tuple)):
                 items = items[0]
-            elif isinstance(items[0],GeneratorType):
+            elif isinstance(items[0], GeneratorType):
                 items = list(items[0])
         super().__init__(items)
 
-    def get(self,name,default=None):
-        return self.name2item.get(name,default)
+    def get(self, name, default=None):
+        return self.name2item.get(name, default)
 
     def names(self):
         return self.name2item.keys()
 
     def get_params(self):
         return self._params
 
@@ -71,45 +86,45 @@
             items.append(item)
         items.name2item = {i.name: i for i in items if isinstance(i, ToolbarItem)}
         items.listing = listing
         return items
 
     def get_context(self):
         # aggregate all items context
-        return RenderContext(*[ i.get_context() for i in self])
+        return RenderContext(*[i.get_context() for i in self])
 
 
 class ToolbarItemMeta(type):
     slug2class = {}
 
     def __new__(mcs, name, bases, attrs):
         cls = super(ToolbarItemMeta, mcs).__new__(mcs, name, bases, attrs)
         ToolbarItemMeta.slug2class[ToolbarItemMeta.get_slug(cls)] = cls
         params_keys = cls.params_keys
-        if isinstance(params_keys,str):
-            params_keys = set(map(str.strip,params_keys.split(',')))
+        if isinstance(params_keys, str):
+            params_keys = set(map(str.strip, params_keys.split(",")))
         TOOLBAR_PARAMS_KEYS.update(params_keys)
-        TOOLBAR_PARAMS_KEYS.discard('')
+        TOOLBAR_PARAMS_KEYS.discard("")
         return cls
 
     @classmethod
     def get_slug(cls, mcs):
-        return mcs.__name__.replace('ToolbarItem','').lower()
+        return mcs.__name__.replace("ToolbarItem", "").lower()
 
     @classmethod
     def get_class(cls, slug):
         return cls.slug2class.get(slug)
 
 
 class ToolbarItem(metaclass=ToolbarItemMeta):
     name = None
-    params_keys = ''
+    params_keys = ""
     attrs = {}
     listing = None
-    theme_button_class = 'btn btn-secondary'
+    theme_button_class = ThemeAttribute("toolbar_theme_button_class")
 
     _ids = count(0)
 
     def __init__(self, *args, **kwargs):
         self.init_args = args
         self.init_kwargs = kwargs
         self.id = next(self._ids)
@@ -119,183 +134,183 @@
 
     def set_listing(self, listing):
         self.listing = listing
 
     def init(self, listing, name=None, **kwargs):
         self.set_listing(listing)
         if name:
-            self.name = re.sub(r'\W','',name)
+            self.name = re.sub(r"\W", "", name)
         if not self.name:
             self.name = ToolbarItemMeta.get_slug(self.__class__)
         self.set_kwargs(**kwargs)
         self.apply_template_kwargs()
-        if not isinstance(self.attrs,HTMLAttributes):
+        if not isinstance(self.attrs, HTMLAttributes):
             self.attrs = HTMLAttributes(self.attrs)
         self.css_class = self.__class__.__name__.lower()
 
     def set_kwargs(self, **kwargs):
         # If toolbar_<toolbarItemclass>_<params> exists in listing attributes :
         # take is as a default value
         for k in TOOLBAR_PARAMS_KEYS:
-            listing_key = 'toolbar_{}'.format(k)
-            if hasattr(self.listing,listing_key):
-                setattr(self,k,getattr(self.listing,listing_key))
+            listing_key = "toolbar_{}".format(k)
+            if hasattr(self.listing, listing_key):
+                setattr(self, k, getattr(self.listing, listing_key))
         for k, v in kwargs.items():
             if k in TOOLBAR_PARAMS_KEYS:
-                setattr(self,k,v)
+                setattr(self, k, v)
         # if parameters given in toolbar : apply them
-        for k, v in self.listing.toolbar.get_params().get(self.name,{}).items():
+        for k, v in self.listing.toolbar.get_params().get(self.name, {}).items():
             if k in TOOLBAR_PARAMS_KEYS:
                 setattr(self, k, v)
         # if parameters given in listing apply them to specified toolbarItem
         for k in TOOLBAR_PARAMS_KEYS:
-            key = 'toolbar_{}__{}'.format(self.name,k)
+            key = "toolbar_{}__{}".format(self.name, k)
             v = getattr(self.listing, key, None)
             if v is not None:
                 setattr(self, k, v)
 
     def apply_template_kwargs(self):
         kwargs = self.listing.get_toolbar_item_kwargs(self.name)
         if kwargs:
             for k, v in kwargs.items():
                 if k in TOOLBAR_PARAMS_KEYS:
-                    if isinstance(v,dict):
-                        prev_value = getattr(self,k,None)
-                        if isinstance(prev_value,dict):
+                    if isinstance(v, dict):
+                        prev_value = getattr(self, k, None)
+                        if isinstance(prev_value, dict):
                             prev_value.update(v)
                             continue
-                    setattr(self,k,v)
+                    setattr(self, k, v)
 
     def get_context(self):
         return {}
 
+
 class SortSelectToolbarItem(ToolbarItem):
-    template_name = 'django_listing/tbi_select.html'
-    params_keys = 'up_arrow,down_arrow,has_submit_button'
+    template_name = ThemeTemplate("tbi_select.html")
+    params_keys = "up_arrow,down_arrow,has_submit_button"
     choices = None
-    up_arrow = ' &#xF106;'
-    down_arrow = ' &#xF107;'
+    up_arrow = " &#xF106;"
+    down_arrow = " &#xF107;"
     has_submit_button = False
-    label = _('Sort by')
-    button_label = _('OK')
-    select_name = 'sort'
+    label = _("Sort by")
+    button_label = _("OK")
+    select_name = "sort"
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
         self.choices = normalize_choices(self.choices)
         if not self.choices:
             self.choices = []
             for c in self.listing.columns:
                 self.choices.append((c.name, c.get_header_value() + self.up_arrow))
-                self.choices.append(('-'+c.name, c.get_header_value() + self.down_arrow))
-
+                self.choices.append(
+                    ("-" + c.name, c.get_header_value() + self.down_arrow)
+                )
 
     def get_context(self):
         # get_context is called at rendering time :
         # this is the way to get the asked value for self.listing.sort
         sorting = self.listing.sort
         self.selected_choices = [
-            (sort_key, label, sort_key==sorting)
-            for sort_key,label in self.choices
+            (sort_key, label, sort_key == sorting) for sort_key, label in self.choices
         ]
         # do not need to return a context
 
 
 class SortDropdownToolbarItem(SortSelectToolbarItem):
-    template_name = 'django_listing/tbi_dropdown.html'
-    label = _('Sort by...')
+    template_name = ThemeTemplate("tbi_dropdown.html")
+    label = _("Sort by...")
 
 
 class VariationsToolbarItem(ToolbarItem):
-    template_name = 'django_listing/tbi_variations.html'
-    params_keys = ['show_labels', 'show_icons', 'labels', 'icons']
-    labels = ''
-    icons = ''
+    template_name = ThemeTemplate("tbi_variations.html")
+    params_keys = ["show_labels", "show_icons", "labels", "icons"]
+    labels = ""
+    icons = ""
     show_labels = False
     show_icons = True
     buttons = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
-        if not hasattr(self.listing,'variations_classes'):
+        if not hasattr(self.listing, "variations_classes"):
             raise InvalidToolbarItem(
-                'Variation toolbar item is only for variations listings '
-                '(subclass of ListingVariations)')
+                "Variation toolbar item is only for variations listings "
+                "(subclass of ListingVariations)"
+            )
         nb_variations = len(self.listing.variations_classes)
-        labels = normalize_list(self.labels,force_length=nb_variations)
-        icons = normalize_list(self.icons,force_length=nb_variations)
+        labels = normalize_list(self.labels, force_length=nb_variations)
+        icons = normalize_list(self.icons, force_length=nb_variations)
         urls = [self.listing.get_url(variation=i) for i in range(nb_variations)]
-        self.buttons = list(zip(
-            urls,
-            labels,
-            icons,
-        ))
+        self.buttons = list(
+            zip(
+                urls,
+                labels,
+                icons,
+            )
+        )
 
 
 class PerPageSelectToolbarItem(ToolbarItem):
-    template_name = 'django_listing/tbi_select.html'
-    params_keys = 'choices'
-    choices = '10,25,50,100,-1:All'
+    template_name = ThemeTemplate("tbi_select.html")
+    params_keys = "choices"
+    choices = "10,25,50,100,-1:All"
     has_submit_button = False
-    label = _('Per page')
-    button_label = _('OK')
-    select_name = 'per_page'
+    label = _("Per page")
+    button_label = _("OK")
+    select_name = "per_page"
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
         self.choices = normalize_choices(self.choices, int_keys=True)
 
     def get_context(self):
         # get_context is called at rendering time :
         # this is the way to get the asked value for self.listing.per_page
         # if per_pages is not in choices : add that choice dynamically
-        per_pages = [ c[0] for c in self.choices ]
+        per_pages = [c[0] for c in self.choices]
         per_page = self.listing.per_page
         if per_pages and per_page not in per_pages:
-            for i,p in enumerate(per_pages):
-                if per_page < p or p==-1:
-                    self.choices.insert(i,[per_page,per_page])
+            for i, p in enumerate(per_pages):
+                if per_page < p or p == -1:
+                    self.choices.insert(i, [per_page, per_page])
                     break
             else:
                 self.choices.append([per_page, per_page])
 
         self.selected_choices = [
-            ( pp, label, per_page == pp)
-            for pp,label in self.choices
+            (pp, label, per_page == pp) for pp, label in self.choices
         ]
-        #do not need to return a context
+        # do not need to return a context
 
 
 class PerPageDropdownToolbarItem(PerPageSelectToolbarItem):
-    template_name = 'django_listing/tbi_dropdown.html'
-    label = _('Per page...')
+    template_name = ThemeTemplate("tbi_dropdown.html")
+    label = _("Per page...")
 
 
 class ExportSelectToolbarItem(ToolbarItem):
-    template_name = 'django_listing/tbi_select.html'
-    choices = [('',_('Choose...'))] + EXPORT_FORMATS
+    template_name = ThemeTemplate("tbi_select.html")
+    choices = [("", _("Choose..."))] + EXPORT_FORMATS
     has_submit_button = True
-    label = 'Export to '
-    button_label = _('OK')
-    select_name = 'export'
+    label = "Export to "
+    button_label = _("OK")
+    select_name = "export"
 
     def init(self, *args, **kwargs):
         super().init(*args, **kwargs)
         self.choices = normalize_choices(self.choices)
-        self.selected_choices = [
-            (key, label, False)
-            for key, label in self.choices
-        ]
+        self.selected_choices = [(key, label, False) for key, label in self.choices]
 
 
 class ExportDropdownToolbarItem(ExportSelectToolbarItem):
-    template_name = 'django_listing/tbi_dropdown.html'
-    label = _('Export to...')
+    template_name = ThemeTemplate("tbi_dropdown.html")
+    label = _("Export to...")
     choices = EXPORT_FORMATS
 
 
 class UpdateToolbarItem(ToolbarItem):
-    template_name = 'django_listing/tbi_update.html'
-    label = _('Update')
+    template_name = ThemeTemplate("tbi_update.html")
+    label = _("Update")
```

### Comparing `django-listing-0.0.9/django_listing/html_attributes.py` & `django-listing-0.5.0/django_listing/html_attributes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 #
 # Created : 2018-02-10
 #
 # @author: Eric Lapouyade
 #
 
-from .exceptions import *
 from django.utils.safestring import mark_safe
 
-__all__ = ['HTMLAttributes']
+__all__ = ["HTMLAttributes"]
+
 
 class HTMLAttributes(dict):
     def __init__(self, *args, **kwargs):
         # remove starting underscore to be able to use '_class'
         # instead of 'class' in kwargs (reserved keyword)
-        if '_class' in kwargs:
-            kwargs['class'] = kwargs.pop('_class')
-        super().__init__(*args,**kwargs)
+        if "_class" in kwargs:
+            kwargs["class"] = kwargs.pop("_class")
+        super().__init__(*args, **kwargs)
 
-    def add(self,attr,value):
+    def add(self, attr, value):
         if value is not None:
             if attr not in self:
                 s = set()
             else:
-                if attr == 'style':
-                    s=set(self[attr].split(';'))
+                if attr == "style":
+                    s = set(self[attr].split(";"))
                 else:
-                    s=set(self[attr].split())
-            if isinstance(value,set):
+                    s = set(self[attr].split())
+            if isinstance(value, set):
                 s.update(value)
             else:
                 s.add(value)
-            if attr == 'style':
-                self[attr] = (';'.join(s)).strip()
+            if attr == "style":
+                self[attr] = (";".join(s)).strip()
             else:
-                self[attr] = (' '.join(s)).strip()
+                self[attr] = (" ".join(s)).strip()
 
     def set(self, attr, value=None):
-        self[attr]=value
+        self[attr] = value
 
     def __setattr__(self, attr, value):
         self[attr] = value
 
     def update(self, *args, **kwargs):
         # remove starting underscore to be able to use '_class'
         # instead of 'class' in kwargs (reserved keyword)
-        if '_class' in kwargs:
-            kwargs['class'] = kwargs.pop('_class')
-        super().update(*args,**kwargs)
+        if "_class" in kwargs:
+            kwargs["class"] = kwargs.pop("_class")
+        super().update(*args, **kwargs)
 
     def copy(self):
         return HTMLAttributes(self)
 
     def __str__(self):
-        out = ' '.join([ ( k if v is None else '{}="{}"'.format(k, v) )
-                        for k, v in self.items()])
+        out = " ".join(
+            [(k if v is None else '{}="{}"'.format(k, v)) for k, v in self.items()]
+        )
         if out:
-            out = ' ' + out
+            out = " " + out
         return mark_safe(out)
```

### Comparing `django-listing-0.0.9/django_listing/actions_buttons_column.py` & `django-listing-0.5.0/django_listing/actions_buttons_column.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,44 +2,75 @@
 # Created : 2020-05-04
 #
 # @author: Eric Lapouyade
 #
 import re
 
 from django.db import models
-from django.db.models import QuerySet
 from django.http import HttpResponse
+from django.middleware.csrf import get_token as get_csrf_token
 from django.template import loader
-from django_listing import Column, InvalidData, ListingException, ModelColumns
-from django.utils.translation import gettext_lazy as _
 from django.utils.translation import gettext
-from django.middleware.csrf import get_token as get_csrf_token
+from django.utils.translation import gettext_lazy as _
+
+from django_listing import Column, ListingException, ModelColumns, InvalidColumn
+
+from .theme_config import ThemeTemplate
+
+__all__ = [
+    "ActionsButtonsColumn",
+]
 
-__all__ = ['ActionsButtonsColumn',]
 
 class ActionsButtonsColumn(Column):
-    params_keys = ( 'buttons', 'buttons_template', 'buttons_text',
-                    'buttons_theme_li_class', 'buttons_theme_button_class',
-                    'buttons_icon', 'buttons_has_icon', 'buttons_has_text')
-    params_keys_suffixes = ('theme_li_class','theme_button_class', 'icon',
-                            'text', 'title', 'has_icon', 'has_text' )
-    buttons = 'move_up,move_down,view_object'
-    buttons_template = 'django_listing/actions_buttons.html'
-    buttons_text = ''
-    buttons_icon = ''
-    buttons_title = ''
+    params_keys = (
+        "buttons",
+        "buttons_has_icon",
+        "buttons_has_text",
+        "buttons_icon",
+        "buttons_template",
+        "buttons_text",
+        "buttons_theme_button_class",
+        "buttons_theme_li_class",
+        "buttons_method",
+        "buttons_url_func",
+    )
+    params_keys_suffixes = (
+        "has_icon",
+        "has_text",
+        "icon",
+        "text",
+        "theme_button_class",
+        "theme_li_class",
+        "title",
+        "method",
+        "url_func",
+    )
+    buttons = "move_up,move_down,view_object,edit_object,delete_object"
+    buttons_template = ThemeTemplate("actions_buttons.html")
+    buttons_text = ""
+    buttons_icon = ""
+    buttons_title = ""
     buttons_has_icon = True
     buttons_has_text = True
-    buttons_theme_li_class = 'action-item'
-    buttons_theme_button_class = 'btn btn-primary'
-    actions_query_string_keys = {'action_col', 'action_button', 'action_pk', }
+    buttons_theme_li_class = "action-item"
+    buttons_theme_button_class = "btn btn-primary"
+    buttons_method = None
+    buttons_url_func = None
+    actions_query_string_keys = {
+        "action_col",
+        "action_button",
+        "action_pk",
+    }
     action_col = None
     action_button = None
     action_pk = None
-    actions_query_string_int_keys = {'action_pk', }
+    actions_query_string_int_keys = {
+        "action_pk",
+    }
     sortable = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.buttons_description = {}
 
     def init(self, *args, **kwargs):
@@ -49,32 +80,32 @@
 
     def render_init(self):
         self.extract_action_params()
 
     def set_kwargs(self, **kwargs):
         super().set_kwargs(**kwargs)
         buttons = self.buttons
-        if isinstance(buttons,str):
-            buttons = set(map(str.strip,buttons.split(',')))
+        if isinstance(buttons, str):
+            buttons = set(map(str.strip, buttons.split(",")))
         suffixes = self.params_keys_suffixes
-        if isinstance(suffixes,str):
-            suffixes = map(str.strip,suffixes.split(','))
-        for k,v in kwargs.items():
-            b, *_ = k.split('__')
+        if isinstance(suffixes, str):
+            suffixes = map(str.strip, suffixes.split(","))
+        for k, v in kwargs.items():
+            b, *_ = k.split("__")
             if b in buttons:
                 setattr(self, k, v)
         for b in buttons:
             description = {}
             for s in suffixes:
-                k = f'{b}__{s}'
-                if hasattr(self,k):
-                    description[s] = getattr(self,k)
+                k = f"{b}__{s}"
+                if hasattr(self, k):
+                    description[s] = getattr(self, k)
                 else:
-                    description[s] = getattr(self,f'buttons_{s}')
-            description['name'] = b
+                    description[s] = getattr(self, f"buttons_{s}")
+            description["name"] = b
             self.buttons_description[b] = description
 
     def extract_action_params(self):
         get_dict = self.listing.request.GET
         post_dict = self.listing.request.POST
         for qs_key in self.actions_query_string_keys:
             v = None
@@ -86,236 +117,299 @@
                 try:
                     v = int(v)
                 except ValueError:
                     pass
             setattr(self, qs_key, v)
 
     def get_buttons_template(self, rec):
-        if not hasattr(self,'_value_template'):
+        if not hasattr(self, "_value_template"):
             self._value_template = loader.get_template(self.buttons_template)
         return self._value_template
 
     def get_buttons_context(self, rec):
         buttons = self.buttons
-        if isinstance(buttons,str):
-            buttons = map(str.strip,buttons.split(','))
+        if isinstance(buttons, str):
+            buttons = map(str.strip, buttons.split(","))
         buttons_context = []
         for b in buttons:
-            meth_name = f'get_button_{b}_context'
+            meth_name = f"get_button_{b}_context"
             context = {}
             context_method = getattr(self.listing, meth_name, None)
             if context_method is not None:
-                context = context_method(self, b, rec)  # give col objet to listing method
+                context = context_method(
+                    self, b, rec
+                )  # give col objet to listing method
             else:
                 context_method = getattr(self, meth_name, None)
                 if context_method is not None:
                     context = context_method(b, rec)
             context.update(
                 self.buttons_description[b],
                 name=b,
-                name_css_class=b.replace('_','-'),
+                name_css_class=b.replace("_", "-"),
             )
             buttons_context.append(context)
         return dict(
             listing=self.listing,
             buttons=buttons_context,
             rec=rec,
             action_col=self.name,
             csrf_token=get_csrf_token(self.listing.request),
         )
 
-    def get_cell_value(self,rec):
+    def get_cell_value(self, rec):
         context = self.get_buttons_context(rec)
         template = self.get_buttons_template(rec)
         return template.render(context)
 
     def get_button_context(self, name, rec):
         return dict(
             name=name,
-            type='submit',
+            type="submit",
         )
 
     def manage_button_action(self, *args, **kwargs):
-        meth_name = f'manage_button_{self.action_button}_action'
+        meth_name = f"manage_button_{self.action_button}_action"
         # Search method in listing object first
         action_method = getattr(self.listing, meth_name, None)
         if action_method is not None:
-            return action_method(self, *args, **kwargs)  # give col objet to listing method
+            return action_method(
+                self, *args, **kwargs
+            )  # give col objet to listing method
         # Search method in column object otherwise
         action_method = getattr(self, meth_name, None)
         if action_method is None:
             raise ListingException(f'Unknown "{self.action_button}" action.')
         return action_method(*args, **kwargs)
 
-    #---------------- MOVE UP --------------------------------------------------
-    move_up__icon = 'listing-icon-up-open'
-    move_up__text = _('Move up')
-    move_up__title = _('Change order up')
-    move_up__field = 'order'
+    def build_url_func_params(self, rec):
+        listing = self.listing
+        if not listing.request:
+            raise ListingException("Listing requires Request object")
+        rm = listing.request.resolver_match
+        return [
+            listing,
+            rec.get_object(),
+            rm.url_name,
+            rm.args,
+            rm.kwargs,
+        ]
+
+    # ---------------- MOVE UP --------------------------------------------------
+    move_up__icon = "listing-icon-up-open"
+    move_up__text = _("Move up")
+    move_up__title = _("Change order up")
+    move_up__field = "order"
 
     def get_button_move_up_context(self, name, rec):
         first = self.listing.records.get_first_obj()
-        is_first = (rec.pk == first.pk)
+        is_first = rec.pk == first.pk
         return dict(
-            type='button' if is_first else 'submit',
+            type="button" if is_first else "submit",
             disabled=is_first,
         )
 
     def manage_button_move_up_action(self, *args, **kwargs):
-        if not isinstance(self.action_pk,int):
-            raise ListingException(f'Bad object Id ({self.action_pk}) '
-                                   f'for action "{self.action_button}"')
+        if not isinstance(self.action_pk, int):
+            raise ListingException(
+                f"Bad object Id ({self.action_pk}) "
+                f'for action "{self.action_button}"'
+            )
         first = self.listing.records.get_first_obj()
         obj = self.listing.records.get_obj(pk=self.action_pk)
         if first and obj:
             field = self.move_up__field
             first_order = getattr(first, field)
             obj_order = getattr(obj, field)
             if first_order < obj_order:
                 self.listing.records.move_obj_order(obj, field, -1)
             elif first_order > obj_order:
                 self.listing.records.move_obj_order(obj, field, 1)
 
-    #---------------- MOVE DOWN ------------------------------------------------
-    move_down__icon = 'listing-icon-down-open'
-    move_down__text = _('Move down')
-    move_down__title = _('Change order down')
-    move_down__field = 'order'
+    # ---------------- MOVE DOWN ------------------------------------------------
+    move_down__icon = "listing-icon-down-open"
+    move_down__text = _("Move down")
+    move_down__title = _("Change order down")
+    move_down__field = "order"
 
     def get_button_move_down_context(self, name, rec):
         last = self.listing.records.get_last_obj()
-        is_last = (rec.pk == last.pk)
+        is_last = rec.pk == last.pk
         return dict(
-            type='button' if is_last else 'submit',
+            type="button" if is_last else "submit",
             disabled=is_last,
         )
 
     def manage_button_move_down_action(self, *args, **kwargs):
-        if not isinstance(self.action_pk,int):
-            raise ListingException(f'Bad object Id ({self.action_pk}) '
-                                   f'for action "{self.action_button}"')
+        if not isinstance(self.action_pk, int):
+            raise ListingException(
+                f"Bad object Id ({self.action_pk}) "
+                f'for action "{self.action_button}"'
+            )
         last = self.listing.records.get_last_obj()
         obj = self.listing.records.get_obj(pk=self.action_pk)
         if last and obj:
             field = self.move_up__field
             last_order = getattr(last, field)
             obj_order = getattr(obj, field)
             if last_order < obj_order:
                 self.listing.records.move_obj_order(obj, field, -1)
             elif last_order > obj_order:
                 self.listing.records.move_obj_order(obj, field, 1)
 
-    #---------------- VIEW OBJECT ----------------------------------------------
-    view_object__icon = 'listing-icon-magnifier'
-    view_object__text = _('Details')
-    view_object__title = _('See details')
+    # ---------------- VIEW OBJECT ----------------------------------------------
+    view_object__icon = "listing-icon-magnifier"
+    view_object__text = _("Details")
+    view_object__title = _("See details")
+    view_object__url_func = None
 
     def get_button_view_object_context(self, name, rec):
-        return dict(
-            type='link',
-            url=rec.get_href()
-        )
+        if self.view_object__url_func:
+            return dict(
+                type="extlink",
+                url=self.view_object__url_func(*self.build_url_func_params(rec)),
+            )
+        return dict(type="extlink", url=rec.get_href())
 
-    #---------------- VIEW OBJECT POPUP ----------------------------------------
-    view_object_popup__icon = 'listing-icon-magnifier'
-    view_object_popup__text = _('Details')
-    view_object_popup__title = _('See details')
-    view_object_popup__template_name = 'django_listing/view_object_popup.html'
-    view_object_popup__layout = ''
-    view_object_popup__label_ending = ' :'
+    # ---------------- EDIT OBJECT ----------------------------------------------
+    edit_object__icon = "listing-icon-pencil"
+    edit_object__text = _("Edit")
+    edit_object__title = _("Edit")
+    edit_object__url_func = None
+    edit_object__method = "get_edit_absolute_url"
+
+    def get_button_edit_object_context(self, name, rec):
+        if self.edit_object__url_func:
+            return dict(
+                type="extlink",
+                url=self.edit_object__url_func(*self.build_url_func_params(rec)),
+            )
+        method = getattr(rec.get_object(), self.edit_object__method, None)
+        if method is None:
+            raise InvalidColumn(
+                f"Please define the method {self.edit_object__method}() "
+                f"in class {rec.get_object().__class__.__name__}"
+            )
+        return dict(type="extlink", url=method())
+
+    # ---------------- DELETE OBJECT ----------------------------------------------
+    delete_object__icon = "listing-icon-trash-empty"
+    delete_object__text = _("Delete")
+    delete_object__title = _("Delete")
+    delete_object__url_func = None
+    delete_object__method = "get_delete_absolute_url"
+
+    def get_button_delete_object_context(self, name, rec):
+        if self.delete_object__url_func:
+            return dict(
+                type="extlink",
+                url=self.delete_object__url_func(*self.build_url_func_params(rec)),
+            )
+        method = getattr(rec.get_object(), self.delete_object__method, None)
+        if method is None:
+            raise InvalidColumn(
+                f"Please define the method {self.delete_object__method}() "
+                f"in class {rec.get_object().__class__.__name__}"
+            )
+        return dict(type="extlink", url=method())
+
+    # ---------------- VIEW OBJECT POPUP ----------------------------------------
+    view_object_popup__icon = "listing-icon-magnifier"
+    view_object_popup__text = _("Details")
+    view_object_popup__title = _("See details")
+    view_object_popup__template_name = ThemeTemplate("view_object_popup.html")
+    view_object_popup__layout = ""
+    view_object_popup__label_ending = " :"
     view_object_popup__display_empty = True
-    view_object_popup__empty_msg = _('Not set')
+    view_object_popup__empty_msg = _("Not set")
 
     def get_button_view_object_popup_context(self, name, rec):
-        return dict(
-            type='link',
-            url='#'  # use jquery
-        )
+        return dict(type="link", url="#")  # use jquery
 
     def get_view_object_popup_template(self):
         return self.view_object_popup__template_name
 
     def get_view_object_popup_layout(self):
-        return str(self.view_object_popup__layout) # str() is important here
+        return str(self.view_object_popup__layout)  # str() is important here
 
     def manage_button_view_object_popup_action(self, *args, **kwargs):
         layout = self.get_view_object_popup_layout()
-        if (not layout or layout.startswith('-')) and self.listing.model:
-            exclude = layout[1:].split(',')
-            layout = ';'.join([f.name
-                for f in self.listing.model._meta.get_fields()
-                if ( not isinstance(f,(models.ManyToManyRel, models.ManyToOneRel))
-                     and f.name not in exclude )
-            ])
+        if (not layout or layout.startswith("-")) and self.listing.model:
+            exclude = layout[1:].split(",")
+            layout = ";".join(
+                [
+                    f.name
+                    for f in self.listing.model._meta.get_fields()
+                    if (
+                        not isinstance(f, (models.ManyToManyRel, models.ManyToOneRel))
+                        and f.name not in exclude
+                    )
+                ]
+            )
         if isinstance(layout, str):
             # transform layout string into list of lists of list
-            layout = list(map(lambda s: s.split(','),layout.split(';')))
+            layout = list(map(lambda s: s.split(","), layout.split(";")))
         else:
-            raise ListingException(gettext('You must specify a layout in '
-                                           'view_object_popup__layout'))
+            raise ListingException(
+                gettext("You must specify a layout in " "view_object_popup__layout")
+            )
         if self.action_pk is None:
-            raise ListingException(gettext('Object id not specified !'))
+            raise ListingException(gettext("Object id not specified !"))
         rec = self.listing.records.get_rec(pk=self.action_pk)
         rows = []
         max_col = 1
         for layout_row in layout:
             cols = []
             for layout_col in layout_row:
-                layout_col, *colspan = layout_col.rsplit('*',1)
+                layout_col, *colspan = layout_col.rsplit("*", 1)
                 layout_col = layout_col.strip()
                 try:
                     # field*2 mean span field onto 2 x (field label + value cell)
                     # So the HTML "colspan" applied on value field needs some calculations
-                    colspan = int(colspan[0].strip())*2 - 1
+                    colspan = int(colspan[0].strip()) * 2 - 1
                 except (ValueError, IndexError):
                     # no colspan attribute
                     colspan = 0
                 if not layout_col:
-                    label = ''
-                    value = ''
-                elif layout_col.startswith('=='):
-                    label = '== section =='
-                    value = re.sub(r'=+\s*(\S.*?\S)\s*=+$',r'\1',layout_col)
+                    label = ""
+                    value = ""
+                elif layout_col.startswith("=="):
+                    label = "== section =="
+                    value = re.sub(r"=+\s*(\S.*?\S)\s*=+$", r"\1", layout_col)
                 else:
                     # layout_col could be 'field' or 'A forced label:field'
-                    if ':' in layout_col:
-                        forced_label, field = layout_col.rsplit(':',1)
+                    if ":" in layout_col:
+                        forced_label, field = layout_col.rsplit(":", 1)
                     else:
                         forced_label, field = None, layout_col
                     col = self.listing.columns.get(field)
                     # if column not defined in listing because not displayed,
                     # create it on-the-fly :
                     if not col and self.listing.model:
-                        col = ModelColumns.create_column_name(
-                            self.listing, field)
+                        col = ModelColumns.create_column_name(self.listing, field)
                     if col:
                         label = forced_label or col.get_header_value()
                         value = col.render_cell(rec)
                     else:
                         label = forced_label or field
-                        value = gettext('*** Not a valid column name ***')
+                        value = gettext("*** Not a valid column name ***")
                 if colspan:
-                    value = re.sub(r'(<td[^>]*)',
-                                   rf'\1 colspan="{colspan}"',
-                                   value, re.I)
+                    value = re.sub(
+                        r"(<td[^>]*)", rf'\1 colspan="{colspan}"', value, re.I
+                    )
                 cols.append((label, value))
 
             rows.append(cols)
             max_col = max(max_col, len(cols))
 
         context = dict(
             object=rec.get_object(),
             rows=rows,
-            full_colspan=max_col*2,
+            full_colspan=max_col * 2,
             action_column=self,
             label_ending=self.view_object_popup__label_ending,
             display_empty=self.view_object_popup__display_empty,
             empty_msg=self.view_object_popup__empty_msg,
         )
         template_name = self.get_view_object_popup_template()
         template = loader.get_template(template_name)
         return HttpResponse(template.render(context))
-
-
-
-
-
```

### Comparing `django-listing-0.0.9/django_listing/paginators.py` & `django-listing-0.5.0/django_listing/paginators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,192 +1,244 @@
 #
 # Created : 2018-02-06
 #
 # @author: Eric Lapouyade
 #
 
 from django.core.paginator import Paginator as DjangoPaginator
-from .context import RenderContext
 from django.utils.translation import pgettext_lazy
 
-__all__ = ['Paginator', 'NoTextButtonPaginator', 'NoTextButtonPaginatorMixin',
-           'NoIconButtonPaginatorMixin','NoIconButtonPaginator']
+from .context import RenderContext
+from .theme_config import ThemeAttribute, ThemeTemplate
+
+__all__ = [
+    "NoIconButtonPaginator",
+    "NoIconButtonPaginatorMixin",
+    "NoTextButtonPaginator",
+    "NoTextButtonPaginatorMixin",
+    "Paginator",
+]
 
 PAGINATOR_PARAMS_KEYS = {
-    'template_name', 'has_page_info', 'page_info_tpl', 'has_prev_next',
-    'has_first_last', 'fast_page_step', 'fast_page_prev_tpl',
-    'fast_page_next_tpl', 'page_scale_size', 'page_scale_ellipsis',
-    'hide_disabled_buttons', 'theme_first_last_has_icon',
-    'theme_first_last_has_text', 'theme_first_icon','theme_last_icon',
-    'theme_fast_page_has_icon', 'theme_fast_page_has_text',
-    'theme_fast_prev_icon', 'theme_fast_next_icon', 'theme_prev_next_has_icon',
-    'theme_prev_next_has_text', 'theme_prev_icon', 'theme_next_icon',
-    'has_row_info', 'page_row_tpl', 'parts_order', 'has_goto_page',
-    'goto_page_tpl', 'has_editable_page_info', 'theme_button_a_class',
-    'theme_button_li_class', 'in_footer', 'hide_single_page',
-    'theme_button_text_class',
+    "fast_page_next_tpl",
+    "fast_page_prev_tpl",
+    "fast_page_step",
+    "goto_page_tpl",
+    "has_editable_page_info",
+    "has_first_last",
+    "has_goto_page",
+    "has_page_info",
+    "has_prev_next",
+    "has_row_info",
+    "hide_disabled_buttons",
+    "hide_single_page",
+    "in_footer",
+    "page_info_tpl",
+    "page_row_tpl",
+    "page_scale_ellipsis",
+    "page_scale_size",
+    "parts_order",
+    "template_name",
+    "theme_button_a_class",
+    "theme_button_li_class",
+    "theme_button_text_class",
+    "theme_fast_next_icon",
+    "theme_fast_page_has_icon",
+    "theme_fast_page_has_text",
+    "theme_fast_prev_icon",
+    "theme_first_icon",
+    "theme_first_last_has_icon",
+    "theme_first_last_has_text",
+    "theme_last_icon",
+    "theme_next_icon",
+    "theme_prev_icon",
+    "theme_prev_next_has_icon",
+    "theme_prev_next_has_text",
 }
 
+
 class Paginator(DjangoPaginator):
-    template_name = 'django_listing/paginator.html'
+    template_name = ThemeTemplate("paginator.html")
     has_page_info = True
     has_editable_page_info = False
-    page_info_tpl = pgettext_lazy('paginator','Page {page_number} of {nb_pages}')
+    page_info_tpl = pgettext_lazy("paginator", "Page {page_number} of {nb_pages}")
     has_row_info = False
-    row_info_tpl = pgettext_lazy('paginator','{row_first}-{row_last} of {nb_rows}')
+    row_info_tpl = pgettext_lazy("paginator", "{row_first}-{row_last} of {nb_rows}")
     has_prev_next = True
-    prev_text = pgettext_lazy('paginator','Previous')
-    next_text = pgettext_lazy('paginator','Next')
+    prev_text = pgettext_lazy("paginator", "Previous")
+    next_text = pgettext_lazy("paginator", "Next")
     has_first_last = False
-    first_text = pgettext_lazy('paginator','First')
-    last_text = pgettext_lazy('paginator','Last')
+    first_text = pgettext_lazy("paginator", "First")
+    last_text = pgettext_lazy("paginator", "Last")
     fast_page_step = 0
-    fast_page_prev_tpl = '-{step}'
-    fast_page_next_tpl = '+{step}'
+    fast_page_prev_tpl = "-{step}"
+    fast_page_next_tpl = "+{step}"
     page_scale_size = 0
     page_scale_ellipsis = 0
     hide_disabled_buttons = False
     hide_single_page = False
-    parts_order = ( 'first,fastprev,prev,pageinfo,rowinfo,scale,'
-                    'next,fastnext,last' )
+    parts_order = "first,fastprev,prev,pageinfo,rowinfo,scale," "next,fastnext,last"
     has_goto_page = False
-    goto_page_tpl = pgettext_lazy('paginator','Go to page {goto_form}')
+    goto_page_tpl = pgettext_lazy("paginator", "Go to page {goto_form}")
     in_footer = False
 
-    theme_first_last_has_icon = True
-    theme_first_last_has_text = True
-    theme_first_icon = 'listing-icon-to-start-1'
-    theme_last_icon = 'listing-icon-to-end-1'
-    theme_fast_page_has_icon = True
-    theme_fast_page_has_text = True
-    theme_fast_prev_icon = 'listing-icon-fast-backward'
-    theme_fast_next_icon = 'listing-icon-fast-forward'
-    theme_prev_next_has_icon = True
-    theme_prev_next_has_text = True
-    theme_prev_icon = 'listing-icon-left-dir'
-    theme_next_icon = 'listing-icon-right-dir'
-    theme_button_a_class = 'page-link'
-    theme_button_li_class = 'page-item'
-    theme_button_text_class = 'button-text'
-
-    def __init__(self, listing, object_list, per_page, orphans=0,
-                 allow_empty_first_page=True):
-        super().__init__(object_list, per_page, orphans,
-                         allow_empty_first_page)
+    theme_first_last_has_icon = ThemeAttribute("paginator_theme_first_last_has_icon")
+    theme_first_last_has_text = ThemeAttribute("paginator_theme_first_last_has_text")
+    theme_first_icon = ThemeAttribute("paginator_theme_first_icon")
+    theme_last_icon = ThemeAttribute("paginator_theme_last_icon")
+    theme_fast_page_has_icon = ThemeAttribute("paginator_theme_fast_page_has_icon")
+    theme_fast_page_has_text = ThemeAttribute("paginator_theme_fast_page_has_text")
+    theme_fast_prev_icon = ThemeAttribute("paginator_theme_fast_prev_icon")
+    theme_fast_next_icon = ThemeAttribute("paginator_theme_fast_next_icon")
+    theme_prev_next_has_icon = ThemeAttribute("paginator_theme_prev_next_has_icon")
+    theme_prev_next_has_text = ThemeAttribute("paginator_theme_prev_next_has_text")
+    theme_prev_icon = ThemeAttribute("paginator_theme_prev_icon")
+    theme_next_icon = ThemeAttribute("paginator_theme_next_icon")
+    theme_button_a_class = ThemeAttribute("paginator_theme_button_a_class")
+    theme_button_li_class = ThemeAttribute("paginator_theme_button_li_class")
+    theme_button_text_class = ThemeAttribute("paginator_theme_button_text_class")
+
+    def __init__(
+        self, listing, object_list, per_page, orphans=0, allow_empty_first_page=True
+    ):
+        super().__init__(object_list, per_page, orphans, allow_empty_first_page)
         self.listing = listing
         for k in PAGINATOR_PARAMS_KEYS:
-            listing_key = 'paginator_' + k
-            if hasattr(listing,listing_key):
-                setattr(self,k,getattr(listing,listing_key))
-        if isinstance(self.parts_order,str):
-            self.parts_order = self.parts_order.replace(' ','')
+            listing_key = "paginator_" + k
+            if hasattr(listing, listing_key):
+                setattr(self, k, getattr(listing, listing_key))
+        if isinstance(self.parts_order, str):
+            self.parts_order = self.parts_order.replace(" ", "")
             self.parts_order = list(
-                map(lambda s:s.split(','),self.parts_order.split(';')))
+                map(lambda s: s.split(","), self.parts_order.split(";"))
+            )
 
     def get_context(self):
         get_url = self.listing.get_url
         page = self.listing.current_page
-        fast_page_prev = max(1, page.number-self.fast_page_step)
-        fast_page_next = min(self.num_pages, page.number+self.fast_page_step)
+        fast_page_prev = max(1, page.number - self.fast_page_step)
+        fast_page_next = min(self.num_pages, page.number + self.fast_page_step)
         beginning_ellipsis_pages = []
         beginning_ellipsis_display = True
         ending_ellipsis_pages = []
         ending_ellipsis_display = True
         if self.page_scale_size:
-            scale_range_min = max(1,page.number-int(self.page_scale_size/2))
-            scale_range_max = min(scale_range_min+self.page_scale_size-1,
-                                  self.num_pages)
+            scale_range_min = max(1, page.number - int(self.page_scale_size / 2))
+            scale_range_max = min(
+                scale_range_min + self.page_scale_size - 1, self.num_pages
+            )
 
             if self.page_scale_ellipsis:
-                beginning_ellipsis_pages = [(p, get_url(page=p), p == page.number)
-                    for p in range(1,min(self.page_scale_ellipsis+1,scale_range_min))]
-                if scale_range_min < self.page_scale_ellipsis+2:
+                beginning_ellipsis_pages = [
+                    (p, get_url(page=p), p == page.number)
+                    for p in range(
+                        1, min(self.page_scale_ellipsis + 1, scale_range_min)
+                    )
+                ]
+                if scale_range_min < self.page_scale_ellipsis + 2:
                     beginning_ellipsis_display = False
                 if scale_range_max == self.num_pages:
-                    scale_range_min = max(1, self.num_pages-self.page_scale_size)
+                    scale_range_min = max(1, self.num_pages - self.page_scale_size)
                 else:
-                    ending_ellipsis_range_min = max(scale_range_max+1,
-                        self.num_pages-self.page_scale_ellipsis+1)
-                    if ending_ellipsis_range_min == scale_range_max+1:
-                        beginning_ellipsis_display=False
+                    ending_ellipsis_range_min = max(
+                        scale_range_max + 1,
+                        self.num_pages - self.page_scale_ellipsis + 1,
+                    )
+                    if ending_ellipsis_range_min == scale_range_max + 1:
+                        beginning_ellipsis_display = False
                     ending_ellipsis_range_max = self.num_pages
-                    ending_ellipsis_pages = [(p,get_url(page=p),p==page.number)
-                        for p in range(ending_ellipsis_range_min,ending_ellipsis_range_max+1)]
-
-            scale_pages = [ (p,get_url(page=p),p==page.number)
-                            for p in range(scale_range_min,scale_range_max+1)]
+                    ending_ellipsis_pages = [
+                        (p, get_url(page=p), p == page.number)
+                        for p in range(
+                            ending_ellipsis_range_min, ending_ellipsis_range_max + 1
+                        )
+                    ]
+
+            scale_pages = [
+                (p, get_url(page=p), p == page.number)
+                for p in range(scale_range_min, scale_range_max + 1)
+            ]
         else:
             scale_pages = []
 
         if self.has_editable_page_info or self.has_goto_page:
             goto_form = '<form class="goto-page">'
-            goto_form += self.listing.get_hiddens_html(without='page')
-            goto_form += ( '<input type="text" '
-                             'value="{val}" '
-                             'name="page{suffix}">'.format(
-                            val = page.number,
-                            suffix=self.listing.suffix))
-            goto_form += '</form>'
+            goto_form += self.listing.get_hiddens_html(without="page")
+            goto_form += (
+                '<input type="text" '
+                'value="{val}" '
+                'name="page{suffix}">'.format(
+                    val=page.number, suffix=self.listing.suffix
+                )
+            )
+            goto_form += "</form>"
         else:
-            goto_form = ''
+            goto_form = ""
 
         if self.has_editable_page_info:
             page_number = goto_form
         else:
             page_number = page.number
 
         nb_page_rows = page.end_index() - page.start_index() + 1
 
         return RenderContext(
             first_page_url=get_url(page=1),
             last_page_url=get_url(page=self.num_pages),
-            prev_page_url=get_url(page=page.previous_page_number()
-               if page.number > 1
-               else 1),
-            next_page_url=get_url(page=page.next_page_number()
-               if page.number < self.num_pages
-               else self.num_pages),
+            prev_page_url=get_url(
+                page=page.previous_page_number() if page.number > 1 else 1
+            ),
+            next_page_url=get_url(
+                page=page.next_page_number()
+                if page.number < self.num_pages
+                else self.num_pages
+            ),
             fast_page_prev_url=get_url(page=fast_page_prev),
             fast_page_next_url=get_url(page=fast_page_next),
-            fast_page_prev_text=self.fast_page_prev_tpl
-                .format(step=self.fast_page_step),
-            fast_page_next_text=self.fast_page_next_tpl
-                .format(step=self.fast_page_step),
+            fast_page_prev_text=self.fast_page_prev_tpl.format(
+                step=self.fast_page_step
+            ),
+            fast_page_next_text=self.fast_page_next_tpl.format(
+                step=self.fast_page_step
+            ),
             scale_pages=scale_pages,
             beginning_ellipsis_pages=beginning_ellipsis_pages,
             beginning_ellipsis_display=beginning_ellipsis_display,
             ending_ellipsis_pages=ending_ellipsis_pages,
             ending_ellipsis_display=ending_ellipsis_display,
             nb_page_rows=nb_page_rows,
-            page_info=self.page_info_tpl.format(page_number=page_number,
-                                                nb_pages=self.num_pages),
-            row_info=self.row_info_tpl.format(row_first=page.start_index(),
-                                              row_last=page.end_index(),
-                                              nb_rows=self.count,
-                                              nb_page_rows=nb_page_rows),
+            page_info=self.page_info_tpl.format(
+                page_number=page_number, nb_pages=self.num_pages
+            ),
+            row_info=self.row_info_tpl.format(
+                row_first=page.start_index(),
+                row_last=page.end_index(),
+                nb_rows=self.count,
+                nb_page_rows=nb_page_rows,
+            ),
             goto_page=self.goto_page_tpl.format(goto_form=goto_form),
-            show_paginator_single_page=(self.num_pages > 1 or
-                                        not self.hide_single_page),
+            show_paginator_single_page=(
+                self.num_pages > 1 or not self.hide_single_page
+            ),
             current_page=page,
             paginator=self,
         )
 
 
 class NoTextButtonPaginatorMixin:
     theme_first_last_has_text = False
     theme_fast_page_has_text = False
     theme_prev_next_has_text = False
 
 
-class NoTextButtonPaginator(NoTextButtonPaginatorMixin,Paginator):
+class NoTextButtonPaginator(NoTextButtonPaginatorMixin, Paginator):
     pass
 
 
 class NoIconButtonPaginatorMixin:
     theme_first_last_has_icon = False
     theme_fast_page_has_icon = False
     theme_prev_next_has_icon = False
 
 
-class NoIconButtonPaginator(NoIconButtonPaginatorMixin,Paginator):
+class NoIconButtonPaginator(NoIconButtonPaginatorMixin, Paginator):
     pass
-
```

### Comparing `django-listing-0.0.9/PKG-INFO` & `django-listing-0.5.0/django_listing.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,183 @@
 Metadata-Version: 2.1
 Name: django-listing
-Version: 0.0.9
+Version: 0.5.0
 Summary: Library for creating HTML listing / table / data grid
 Home-page: https://github.com/elapouya/django-listing
 Author: Eric Lapouyade
 Author-email: elapouya@gmail.com
 License: GPLv3+
-Description: 
-        ==============
-        django-listing
-        ==============
-        
-        .. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro1.png
-        .. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro2.png
-        
-        Django app for building HTML listings / tables, it includes many features :
-        
-        * Any iterable, Django QuerySet or model can be used.
-        * Most listings can be configured into a template file without touching a python file
-        * A class-based ListingView is provided if you want to code a listing at python side
-        * It as an Ajax mode to save requests to the server
-        * Uses JQuery if ajax is activated
-        * Customized for Bootstrap by default, but can be easily customized in many way (templates, icons, etc...)
-        * You can select columns to display, columns title, default sorting etc..
-        * Pagination is highly customizable (buttons to display, goto page, ellipsis, icons et labels)
-        * Rows can be <div> instead of <tr>, so it is possible to format data in many ways
-        * A lot of column types are provided, they are automatically created when a
-          QuerySet or a model is provided
-        * Columns are class-bases and one can create custom ones
-        * Columns manage One-to-many, Many-to-many and foreign relations
-        * Provides aggregation columns : sum, avg, min, max values
-        * Provides page-level and global aggregation : sum, avg, min, max values displayed at listing last row
-        * Provides columns to make a link to the object, a custom link, checkbox, select box, text input...
-        * Provides "action column" that comes with many actions : show, edit, delete, move up, move down...
-        * is able to manage multiple variations to present data in multiple way at the same place
-          (text only listing, text+image listing, image only listing for example)
-        * Uses Django translation framework : one can translate the listing as needed
-        * Toolbars can be added at the top and/or at the bottom to make actions
-        * Built-in toolbar action are : sorting, select a listing variation, number of rows per page,
-          export data. They are customizable.
-        * Toolbar items are class-based : one can create a custom one easily
-        * django-listing can automatically create a filter form (aka search form)
-        * Listing rows can be selectable in order to apply some actions
-        * Listings can be editable for mass updates
-        * django-listing can automatically create a form for inserting data to database
-        * One can upload files/images into a listing, it uses DropzoneJS (Work in progress)
-        * ListingView can manage itself database inserting, editing, deleting, filtering, uploads and actions :
-          no need to develop any code for that.
-        * django-listing comes with hundreds of icons as a scalable font
-        * django-listing is faster than django-table2
-        
-        
-        Demo
-        ----
-        
-        If you have docker you can run the demo with this command::
-        
-            docker run -p 8123:8123 elapouya/django-listing-demo
-        
-        And then open your browser at this url : http://localhost:8123
-        
-        To install docker on Linux, just use this command::
-        
-            curl -sSL https://get.docker.com/ | sh
-        
-        Otherwise, you can upload from here : https://docs.docker.com/get-docker/
-        
-        Code
-        ....
-        
-        The demo code is available on github here : `django-listing-demo <https://github.com/elapouya/django-listing-demo>`_
-        
-        
-        License
-        -------
-        Django-listing is licensed under the GPLv3 license for all open source applications.
-        A commercial license is required for all commercial applications or non-open applications
-        
-        See `LICENSE.rst <https://github.com/elapouya/django-listing/blob/master/LICENSE.rst>`_ file for more informations.
-        
-        
-        Documentation
-        -------------
-        
-        Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
-        
-        News
-        ----
-        
-        0.0.9 (2021-11-09)
-        ------------------
-        - Add possibility to create custom action button linked with listing method
-        
-        0.0.7 (2020-07-14)
-        ------------------
-        - First running version
-        
-        0.0.1 (2018-02-03)
-        ------------------
-        - Skeleton commit
-        
-        
 Keywords: table,datatable,listing,data grid
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+License-File: LICENSE.rst
+
+
+==============
+django-listing
+==============
+
+.. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro1.png
+.. image:: https://raw.githubusercontent.com/elapouya/django-listing/master/docs/_static/readme_intro2.png
+
+Django app for building HTML listings / tables, it includes many features :
+
+* Any iterable, Django QuerySet or model can be used.
+* Most listings can be configured into a template file without touching a python file
+* A class-based ListingView is provided if you want to code a listing at python side
+* It as an Ajax mode to save requests to the server
+* Uses JQuery if ajax is activated
+* Customized for Bootstrap by default, but can be easily customized in many way (templates, icons, etc...)
+* You can select columns to display, columns title, default sorting etc..
+* Pagination is highly customizable (buttons to display, goto page, ellipsis, icons et labels)
+* Rows can be <div> instead of <tr>, so it is possible to format data in many ways
+* A lot of column types are provided, they are automatically created when a
+  QuerySet or a model is provided
+* Columns are class-bases and one can create custom ones
+* Columns manage One-to-many, Many-to-many and foreign relations
+* Provides aggregation columns : sum, avg, min, max values
+* Provides page-level and global aggregation : sum, avg, min, max values displayed at listing last row
+* Provides columns to make a link to the object, a custom link, checkbox, select box, text input...
+* Provides "action column" that comes with many actions : show, edit, delete, move up, move down...
+* is able to manage multiple variations to present data in multiple way at the same place
+  (text only listing, text+image listing, image only listing for example)
+* Uses Django translation framework : one can translate the listing as needed
+* Toolbars can be added at the top and/or at the bottom to make actions
+* Built-in toolbar action are : sorting, select a listing variation, number of rows per page,
+  export data. They are customizable.
+* Toolbar items are class-based : one can create a custom one easily
+* django-listing can automatically create a filter form (aka search form)
+* Listing rows can be selectable in order to apply some actions
+* Listings can be editable for mass updates
+* django-listing can automatically create a form for inserting data to database
+* One can upload files/images into a listing, it uses DropzoneJS (Work in progress)
+* ListingView can manage itself database inserting, editing, deleting, filtering, uploads and actions :
+  no need to develop any code for that.
+* django-listing comes with hundreds of icons as a scalable font
+* django-listing is faster than django-table2
+
+
+Showcase
+--------
+
+A demo is included in source code, you will need `poetry <https://python-poetry.org/docs/>`_ to install python environment::
+
+    curl -sSL https://install.python-poetry.org | python3 -
+
+To install the python envionment, go to django-listing source code root directory, then::
+
+    cd showcase
+    poetry install
+
+Check you are in ``showcase/`` directory, then start the Django from poetry environment::
+
+    poetry run python manage.py runserver 8123
+
+A sqlite database is already included, you do not have to make any migration,
+just open your brower at http://localhost:8123
+
+
+License
+-------
+Django-listing is licensed under the GPLv3 license for all open source applications.
+A commercial license is required for all commercial applications or non-open applications
+
+See `LICENSE.rst <https://github.com/elapouya/django-listing/blob/master/LICENSE.rst>`_ file for more informations.
+
+
+Documentation
+-------------
+
+Please, `read the doc <http://django-listing.readthedocs.org>`_  (Work in progress)
+
+News
+----
+
+0.5.0 (2023-07-05)
+------------------
+- Add __url_func parameter for edit/delete/view action buttons
+
+0.0.28 (2023-06-27)
+-------------------
+- Add AutocompleteMultipleForeignKeyFilter
+
+0.0.27 (2023-06-26)
+-------------------
+- Add ForeignKeyFilter and AutocompleteForeignKeyFilter
+
+0.0.26 (2023-06-21)
+-------------------
+- Added edit and delete action buttons
+- Fixed action button "see details" modal
+
+0.0.24 (2023-06-20)
+-------------------
+- Improved CSS for small device
+- Auto-detect many-to-many model fields if present in select_columns
+
+0.0.23 (2023-06-19)
+-------------------
+- Fixed choices widgets
+
+0.0.22 (2023-06-19)
+-------------------
+- Improved radio and checkbox in filter form
+
+0.0.21 (2023-06-15)
+-------------------
+- Fixed ModelColumns
+
+0.0.20 (2023-05-19)
+-------------------
+- Added LineNumberColumn()
+
+0.0.18 (2023-05-05)
+-------------------
+- Use scss to generate css files
+
+0.0.17 (2023-04-26)
+-------------------
+- Added showcase with many demo pages see showcase/README.rst
+
+0.0.14 (2022-10-24)
+-------------------
+- Fixed bad form closing
+- Fixed ListingVariation with Ajax
+
+0.0.12 (2022-07-04)
+-------------------
+- Added django-like filter syntax for sequences
+
+0.0.11 (2022-06-02)
+-------------------
+- Added JsonDateTimeColumn class
+
+0.0.10 (2022-05-17)
+-------------------
+- Added support for python 3.10
+
+0.0.9 (2021-11-09)
+------------------
+- Added possibility to create custom action button linked with listing method
+
+0.0.7 (2020-07-14)
+------------------
+- First running version
+
+0.0.1 (2018-02-03)
+------------------
+- Skeleton commit
+
```

### Comparing `django-listing-0.0.9/README.rst` & `django-listing-0.5.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -38,33 +38,32 @@
 * One can upload files/images into a listing, it uses DropzoneJS (Work in progress)
 * ListingView can manage itself database inserting, editing, deleting, filtering, uploads and actions :
   no need to develop any code for that.
 * django-listing comes with hundreds of icons as a scalable font
 * django-listing is faster than django-table2
 
 
-Demo
-----
+Showcase
+--------
 
-If you have docker you can run the demo with this command::
+A demo is included in source code, you will need `poetry <https://python-poetry.org/docs/>`_ to install python environment::
 
-    docker run -p 8123:8123 elapouya/django-listing-demo
+    curl -sSL https://install.python-poetry.org | python3 -
 
-And then open your browser at this url : http://localhost:8123
+To install the python envionment, go to django-listing source code root directory, then::
 
-To install docker on Linux, just use this command::
+    cd showcase
+    poetry install
 
-    curl -sSL https://get.docker.com/ | sh
+Check you are in ``showcase/`` directory, then start the Django from poetry environment::
 
-Otherwise, you can upload from here : https://docs.docker.com/get-docker/
+    poetry run python manage.py runserver 8123
 
-Code
-....
-
-The demo code is available on github here : `django-listing-demo <https://github.com/elapouya/django-listing-demo>`_
+A sqlite database is already included, you do not have to make any migration,
+just open your brower at http://localhost:8123
 
 
 License
 -------
 Django-listing is licensed under the GPLv3 license for all open source applications.
 A commercial license is required for all commercial applications or non-open applications
```

