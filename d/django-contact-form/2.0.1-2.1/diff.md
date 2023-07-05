# Comparing `tmp/django-contact-form-2.0.1.tar.gz` & `tmp/django-contact-form-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-contact-form-2.0.1.tar", last modified: Tue May 31 05:52:14 2022, max compression
+gzip compressed data, was "django-contact-form-2.1.tar", last modified: Wed Jul  5 06:29:24 2023, max compression
```

## Comparing `django-contact-form-2.0.1.tar` & `django-contact-form-2.1.tar`

### file list

```diff
@@ -1,82 +1,87 @@
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.832110 django-contact-form-2.0.1/
--rw-r--r--   0 james      (503) staff       (20)     1523 2022-05-30 06:56:29.000000 django-contact-form-2.0.1/LICENSE
--rw-r--r--   0 james      (503) staff       (20)      135 2018-09-10 01:57:28.000000 django-contact-form-2.0.1/MANIFEST.in
--rw-r--r--   0 james      (503) staff       (20)     1493 2022-05-31 05:52:14.832367 django-contact-form-2.0.1/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)      478 2020-12-12 09:41:33.000000 django-contact-form-2.0.1/README.rst
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.813609 django-contact-form-2.0.1/docs/
--rw-r--r--   0 james      (503) staff       (20)     5616 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/docs/Makefile
--rw-r--r--   0 james      (503) staff       (20)     1294 2022-05-31 05:47:29.000000 django-contact-form-2.0.1/docs/conf.py
--rw-r--r--   0 james      (503) staff       (20)     5078 2022-05-31 05:29:31.000000 django-contact-form-2.0.1/docs/faq.rst
--rw-r--r--   0 james      (503) staff       (20)     9209 2022-05-31 05:18:54.000000 django-contact-form-2.0.1/docs/forms.rst
--rw-r--r--   0 james      (503) staff       (20)      867 2022-05-31 05:07:49.000000 django-contact-form-2.0.1/docs/index.rst
--rw-r--r--   0 james      (503) staff       (20)     2121 2022-05-31 05:22:46.000000 django-contact-form-2.0.1/docs/install.rst
--rw-r--r--   0 james      (503) staff       (20)     5122 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/docs/make.bat
--rw-r--r--   0 james      (503) staff       (20)     6036 2022-05-31 04:51:14.000000 django-contact-form-2.0.1/docs/quickstart.rst
--rw-r--r--   0 james      (503) staff       (20)      107 2018-09-09 08:47:05.000000 django-contact-form-2.0.1/docs/spelling_wordlist.txt
--rw-r--r--   0 james      (503) staff       (20)     2319 2022-05-31 05:46:49.000000 django-contact-form-2.0.1/docs/upgrade.rst
--rw-r--r--   0 james      (503) staff       (20)     3199 2022-05-31 04:55:29.000000 django-contact-form-2.0.1/docs/views.rst
--rw-r--r--   0 james      (503) staff       (20)     2604 2022-05-31 04:41:59.000000 django-contact-form-2.0.1/runtests.py
--rw-r--r--   0 james      (503) staff       (20)      387 2022-05-31 05:52:14.833334 django-contact-form-2.0.1/setup.cfg
--rw-r--r--   0 james      (503) staff       (20)     1384 2022-05-31 05:47:29.000000 django-contact-form-2.0.1/setup.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.800071 django-contact-form-2.0.1/src/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.816069 django-contact-form-2.0.1/src/django_contact_form/
--rw-r--r--   0 james      (503) staff       (20)        0 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/src/django_contact_form/__init__.py
--rw-r--r--   0 james      (503) staff       (20)      708 2022-05-31 04:37:32.000000 django-contact-form-2.0.1/src/django_contact_form/akismet_urls.py
--rw-r--r--   0 james      (503) staff       (20)     5132 2022-05-31 04:56:48.000000 django-contact-form-2.0.1/src/django_contact_form/forms.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.804051 django-contact-form-2.0.1/src/django_contact_form/locale/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.800716 django-contact-form-2.0.1/src/django_contact_form/locale/da/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.819654 django-contact-form-2.0.1/src/django_contact_form/locale/da/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)     1019 2020-02-09 10:11:31.000000 django-contact-form-2.0.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.801204 django-contact-form-2.0.1/src/django_contact_form/locale/de/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.820726 django-contact-form-2.0.1/src/django_contact_form/locale/de/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      532 2018-09-10 05:35:10.000000 django-contact-form-2.0.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      895 2019-12-15 18:19:12.000000 django-contact-form-2.0.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.801617 django-contact-form-2.0.1/src/django_contact_form/locale/en/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.821652 django-contact-form-2.0.1/src/django_contact_form/locale/en/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      378 2018-09-10 05:35:10.000000 django-contact-form-2.0.1/src/django_contact_form/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      796 2018-09-10 05:34:39.000000 django-contact-form-2.0.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.802038 django-contact-form-2.0.1/src/django_contact_form/locale/es/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.822568 django-contact-form-2.0.1/src/django_contact_form/locale/es/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      560 2018-09-10 05:35:10.000000 django-contact-form-2.0.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      891 2018-09-10 05:34:39.000000 django-contact-form-2.0.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.802495 django-contact-form-2.0.1/src/django_contact_form/locale/eu/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.823551 django-contact-form-2.0.1/src/django_contact_form/locale/eu/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      564 2018-09-10 05:35:10.000000 django-contact-form-2.0.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      895 2018-09-10 05:34:39.000000 django-contact-form-2.0.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.802894 django-contact-form-2.0.1/src/django_contact_form/locale/fr/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.824543 django-contact-form-2.0.1/src/django_contact_form/locale/fr/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      530 2018-09-10 05:35:10.000000 django-contact-form-2.0.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      887 2019-12-15 18:19:12.000000 django-contact-form-2.0.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.803335 django-contact-form-2.0.1/src/django_contact_form/locale/it/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.825025 django-contact-form-2.0.1/src/django_contact_form/locale/it/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      726 2018-09-18 14:46:02.000000 django-contact-form-2.0.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.803779 django-contact-form-2.0.1/src/django_contact_form/locale/nl/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.826188 django-contact-form-2.0.1/src/django_contact_form/locale/nl/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      651 2020-09-21 07:57:57.000000 django-contact-form-2.0.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)     1025 2020-09-21 07:57:57.000000 django-contact-form-2.0.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.804213 django-contact-form-2.0.1/src/django_contact_form/locale/uk/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.827314 django-contact-form-2.0.1/src/django_contact_form/locale/uk/LC_MESSAGES/
--rw-r--r--   0 james      (503) staff       (20)      684 2020-02-09 10:11:31.000000 django-contact-form-2.0.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 james      (503) staff       (20)      934 2020-02-09 10:11:31.000000 django-contact-form-2.0.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 james      (503) staff       (20)      601 2022-05-31 04:35:57.000000 django-contact-form-2.0.1/src/django_contact_form/urls.py
--rw-r--r--   0 james      (503) staff       (20)      913 2022-05-31 04:43:42.000000 django-contact-form-2.0.1/src/django_contact_form/views.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.819119 django-contact-form-2.0.1/src/django_contact_form.egg-info/
--rw-r--r--   0 james      (503) staff       (20)     1493 2022-05-31 05:52:14.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/PKG-INFO
--rw-r--r--   0 james      (503) staff       (20)     1972 2022-05-31 05:52:14.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/SOURCES.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2022-05-31 05:52:14.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/dependency_links.txt
--rw-r--r--   0 james      (503) staff       (20)        1 2022-05-31 05:52:12.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/not-zip-safe
--rw-r--r--   0 james      (503) staff       (20)       31 2022-05-31 05:52:14.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/requires.txt
--rw-r--r--   0 james      (503) staff       (20)       20 2022-05-31 05:52:14.000000 django-contact-form-2.0.1/src/django_contact_form.egg-info/top_level.txt
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.829232 django-contact-form-2.0.1/tests/
--rw-r--r--   0 james      (503) staff       (20)        0 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/__init__.py
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.804886 django-contact-form-2.0.1/tests/templates/
-drwxr-xr-x   0 james      (503) staff       (20)        0 2022-05-31 05:52:14.831674 django-contact-form-2.0.1/tests/templates/django_contact_form/
--rw-r--r--   0 james      (503) staff       (20)       11 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/templates/django_contact_form/contact_form.html
--rw-r--r--   0 james      (503) staff       (20)       10 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/templates/django_contact_form/contact_form.txt
--rw-r--r--   0 james      (503) staff       (20)       21 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/templates/django_contact_form/contact_form_sent.html
--rw-r--r--   0 james      (503) staff       (20)       20 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/templates/django_contact_form/contact_form_subject.txt
--rw-r--r--   0 james      (503) staff       (20)       29 2015-12-01 10:34:46.000000 django-contact-form-2.0.1/tests/templates/django_contact_form/test_callable_template_name.html
--rw-r--r--   0 james      (503) staff       (20)     6265 2022-05-31 04:57:19.000000 django-contact-form-2.0.1/tests/test_forms.py
--rw-r--r--   0 james      (503) staff       (20)      823 2022-05-31 04:36:06.000000 django-contact-form-2.0.1/tests/test_urls.py
--rw-r--r--   0 james      (503) staff       (20)     4388 2022-05-31 04:37:19.000000 django-contact-form-2.0.1/tests/test_views.py
--rw-r--r--   0 james      (503) staff       (20)     6701 2022-05-31 04:34:44.000000 django-contact-form-2.0.1/tox.ini
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.906338 django-contact-form-2.1/
+-rw-r--r--   0 james      (503) staff       (20)      299 2023-07-04 01:51:37.000000 django-contact-form-2.1/.editorconfig
+-rw-r--r--   0 james      (503) staff       (20)      107 2023-07-04 01:51:49.000000 django-contact-form-2.1/.flake8
+-rw-r--r--   0 james      (503) staff       (20)     1041 2023-07-04 08:19:03.000000 django-contact-form-2.1/.pre-commit-config.yaml
+-rw-r--r--   0 james      (503) staff       (20)      295 2023-07-04 01:59:19.000000 django-contact-form-2.1/.readthedocs.yaml
+-rw-r--r--   0 james      (503) staff       (20)     1523 2022-05-30 06:56:29.000000 django-contact-form-2.1/LICENSE
+-rw-r--r--   0 james      (503) staff       (20)      293 2023-07-04 08:10:13.000000 django-contact-form-2.1/MANIFEST.in
+-rw-r--r--   0 james      (503) staff       (20)     1710 2023-07-05 06:29:24.906225 django-contact-form-2.1/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)      478 2020-12-12 09:41:33.000000 django-contact-form-2.1/README.rst
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.901949 django-contact-form-2.1/docs/
+-rw-r--r--   0 james      (503) staff       (20)     5616 2015-12-01 10:34:46.000000 django-contact-form-2.1/docs/Makefile
+-rw-r--r--   0 james      (503) staff       (20)     1720 2023-07-05 02:38:57.000000 django-contact-form-2.1/docs/conf.py
+-rw-r--r--   0 james      (503) staff       (20)      106 2023-07-04 01:59:07.000000 django-contact-form-2.1/docs/docs_settings.py
+-rw-r--r--   0 james      (503) staff       (20)     5794 2023-07-05 00:51:40.000000 django-contact-form-2.1/docs/faq.rst
+-rw-r--r--   0 james      (503) staff       (20)      583 2023-07-05 00:25:12.000000 django-contact-form-2.1/docs/forms.rst
+-rw-r--r--   0 james      (503) staff       (20)      868 2023-07-05 00:48:50.000000 django-contact-form-2.1/docs/index.rst
+-rw-r--r--   0 james      (503) staff       (20)     3482 2023-07-05 00:50:19.000000 django-contact-form-2.1/docs/install.rst
+-rw-r--r--   0 james      (503) staff       (20)     5122 2015-12-01 10:34:46.000000 django-contact-form-2.1/docs/make.bat
+-rw-r--r--   0 james      (503) staff       (20)     6040 2023-07-05 00:41:36.000000 django-contact-form-2.1/docs/quickstart.rst
+-rw-r--r--   0 james      (503) staff       (20)      107 2018-09-09 08:47:05.000000 django-contact-form-2.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 james      (503) staff       (20)     2352 2023-07-05 01:59:23.000000 django-contact-form-2.1/docs/upgrade.rst
+-rw-r--r--   0 james      (503) staff       (20)      113 2023-07-05 00:36:23.000000 django-contact-form-2.1/docs/views.rst
+-rw-r--r--   0 james      (503) staff       (20)    10866 2023-07-04 08:13:40.000000 django-contact-form-2.1/noxfile.py
+-rw-r--r--   0 james      (503) staff       (20)     2205 2023-07-04 08:36:59.000000 django-contact-form-2.1/pyproject.toml
+-rw-r--r--   0 james      (503) staff       (20)      364 2023-07-04 08:18:23.000000 django-contact-form-2.1/runtests.py
+-rw-r--r--   0 james      (503) staff       (20)       38 2023-07-05 06:29:24.906374 django-contact-form-2.1/setup.cfg
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897444 django-contact-form-2.1/src/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.902478 django-contact-form-2.1/src/django_contact_form/
+-rw-r--r--   0 james      (503) staff       (20)       77 2023-07-05 06:24:43.000000 django-contact-form-2.1/src/django_contact_form/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)      708 2022-05-31 04:37:32.000000 django-contact-form-2.1/src/django_contact_form/akismet_urls.py
+-rw-r--r--   0 james      (503) staff       (20)    12612 2023-07-05 00:25:05.000000 django-contact-form-2.1/src/django_contact_form/forms.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898504 django-contact-form-2.1/src/django_contact_form/locale/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897607 django-contact-form-2.1/src/django_contact_form/locale/da/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903138 django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)     1019 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897716 django-contact-form-2.1/src/django_contact_form/locale/de/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903401 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      532 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      895 2019-12-15 18:19:12.000000 django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897836 django-contact-form-2.1/src/django_contact_form/locale/en/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903651 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      378 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      796 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.897953 django-contact-form-2.1/src/django_contact_form/locale/es/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903902 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      560 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      891 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898068 django-contact-form-2.1/src/django_contact_form/locale/eu/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904158 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      564 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      895 2018-09-10 05:34:39.000000 django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898190 django-contact-form-2.1/src/django_contact_form/locale/fr/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904389 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      530 2018-09-10 05:35:10.000000 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      887 2019-12-15 18:19:12.000000 django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898307 django-contact-form-2.1/src/django_contact_form/locale/it/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904501 django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      726 2018-09-18 14:46:02.000000 django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898429 django-contact-form-2.1/src/django_contact_form/locale/nl/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904738 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      651 2020-09-21 07:57:57.000000 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)     1025 2020-09-21 07:57:57.000000 django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898557 django-contact-form-2.1/src/django_contact_form/locale/uk/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.904963 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 james      (503) staff       (20)      684 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 james      (503) staff       (20)      934 2020-02-09 10:11:31.000000 django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 james      (503) staff       (20)      601 2022-05-31 04:35:57.000000 django-contact-form-2.1/src/django_contact_form/urls.py
+-rw-r--r--   0 james      (503) staff       (20)     4212 2023-07-05 00:36:19.000000 django-contact-form-2.1/src/django_contact_form/views.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.903030 django-contact-form-2.1/src/django_contact_form.egg-info/
+-rw-r--r--   0 james      (503) staff       (20)     1710 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/PKG-INFO
+-rw-r--r--   0 james      (503) staff       (20)     2029 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (503) staff       (20)        1 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (503) staff       (20)      232 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/requires.txt
+-rw-r--r--   0 james      (503) staff       (20)       20 2023-07-05 06:29:24.000000 django-contact-form-2.1/src/django_contact_form.egg-info/top_level.txt
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.905501 django-contact-form-2.1/tests/
+-rw-r--r--   0 james      (503) staff       (20)        0 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/__init__.py
+-rw-r--r--   0 james      (503) staff       (20)     1399 2023-07-04 02:16:34.000000 django-contact-form-2.1/tests/settings.py
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.898749 django-contact-form-2.1/tests/templates/
+drwxr-xr-x   0 james      (503) staff       (20)        0 2023-07-05 06:29:24.906066 django-contact-form-2.1/tests/templates/django_contact_form/
+-rw-r--r--   0 james      (503) staff       (20)       11 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form.html
+-rw-r--r--   0 james      (503) staff       (20)       10 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form.txt
+-rw-r--r--   0 james      (503) staff       (20)       21 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form_sent.html
+-rw-r--r--   0 james      (503) staff       (20)       20 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/contact_form_subject.txt
+-rw-r--r--   0 james      (503) staff       (20)       29 2015-12-01 10:34:46.000000 django-contact-form-2.1/tests/templates/django_contact_form/test_callable_template_name.html
+-rw-r--r--   0 james      (503) staff       (20)     7287 2023-07-04 08:15:11.000000 django-contact-form-2.1/tests/test_forms.py
+-rw-r--r--   0 james      (503) staff       (20)      823 2022-05-31 04:36:06.000000 django-contact-form-2.1/tests/test_urls.py
+-rw-r--r--   0 james      (503) staff       (20)     4576 2023-07-04 08:09:38.000000 django-contact-form-2.1/tests/test_views.py
```

### Comparing `django-contact-form-2.0.1/LICENSE` & `django-contact-form-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/PKG-INFO` & `django-contact-form-2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: django-contact-form
-Version: 2.0.1
+Version: 2.1
 Summary: A generic contact-form application for Django
-Home-page: https://github.com/ubernostrum/django-contact-form/
-Author: James Bennett
-Author-email: james@b-list.org
+Author-email: James Bennett <james@b-list.org>
+License: BSD-3-Clause
+Project-URL: documentation, https://django-contact-form.readthedocs.io/
+Project-URL: homepage, https://github.com/ubernostrum/django-contact-form
 Keywords: django,email,contact-form
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: akismet
+Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
 
 .. -*-restructuredtext-*-
 
 .. image:: https://github.com/ubernostrum/django-contact-form/workflows/CI/badge.svg
    :alt: CI status image
    :target: https://github.com/ubernostrum/django-contact-form/actions?query=workflow%3ACI
```

### Comparing `django-contact-form-2.0.1/docs/Makefile` & `django-contact-form-2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/docs/conf.py` & `django-contact-form-2.1/docs/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,68 @@
+"""
+Configuration file for the Sphinx documentation builder:
+
+https://www.sphinx-doc.org/
+
+"""
 import os
 import sys
 
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import django_contact_form
 
-extensions = ["sphinx.ext.intersphinx"]
+extensions = [
+    "notfound.extension",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.viewcode",
+    "sphinxcontrib_django",
+    "sphinxext.opengraph",
+    "sphinx_copybutton",
+    "sphinx_inline_tabs",
+]
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "django-contact-form"
-copyright = "2007-2022, James Bennett"
-version = "2.0"
-release = "2.0.1"
+copyright = "2007, James Bennett"
+version = django_contact_form.__version__
+release = django_contact_form.__version__
 exclude_trees = ["_build"]
 pygments_style = "sphinx"
 htmlhelp_basename = "django-contact-formdoc"
+html_theme = "furo"
 latex_documents = [
     (
         "index",
         "django-contact-form.tex",
         "django-contact-form Documentation",
         "James Bennett",
         "manual",
-    ),
+    )
 ]
 
 intersphinx_mapping = {
     "django": (
         "https://docs.djangoproject.com/en/stable/",
         "https://docs.djangoproject.com/en/stable/_objects/",
     ),
     "python": ("https://docs.python.org/3", None),
 }
 
-if not on_rtd:
-    import sphinx_rtd_theme
-
-    html_theme = "sphinx_rtd_theme"
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-
 # Spelling check needs an additional module that is not installed by default.
 # Add it only if spelling check is requested so docs can be generated without it.
 if "spelling" in sys.argv:
     extensions.append("sphinxcontrib.spelling")
 
 # Spelling language.
 spelling_lang = "en_US"
 
 # Location of word list.
 spelling_word_list_filename = "spelling_wordlist.txt"
+
+# OGP metadata configuration.
+ogp_enable_meta_description = True
+ogp_site_url = "https://django-contact-form.readthedocs.io/"
+
+# Django settings for sphinxcontrib-django.
+sys.path.insert(0, os.path.abspath("."))
+django_settings = "docs_settings"
```

### Comparing `django-contact-form-2.0.1/docs/faq.rst` & `django-contact-form-2.1/docs/faq.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,131 @@
 .. _faq:
 
 
 Frequently asked questions
 ==========================
 
-The following notes answer some common questions, and may be useful to
-you when installing, configuring or using django-contact-form.
+The following notes answer some common questions, and may be useful to you when
+installing, configuring or using django-contact-form.
 
 
 What versions of Django and Python are supported?
 -------------------------------------------------
 
-As of django-contact-form |release|, Django 3.2 and 4.0 are
-supported, on Python 3.7 (Django 3.2 only), 3.8, 3.9, and 3.10. Note
-that Django 3.2's support for Python 3.10 was added in Django 3.2.9,
-so you may experience issues with Python 3.10 and earlier Django 3.2
-versions.
+django-contact-form |release| supports Django 3.2, 4.1, and 4.2 on Python 3.8,
+3.9, 3.10, and 3.11 (Django 4.1 and 4.2 only). Note that Django 3.2's support
+for Python 3.10 was added in Django 3.2.9, so you may experience issues with
+Python 3.10 and earlier Django 3.2 versions.
+
+.. note:: **Django 3.2 and supported Python versions**
+
+   Django 3.2 was released before Python 3.10 had come out, and although it now
+   supports Python 3.10, it did not officially do so until the Django 3.2.9
+   release. You may encounter problems if you try to use Django 3.2.8 or
+   earlier with Python 3.10.
+
+   Also, although Django 3.2 continues to officially support Python 3.6 and
+   3.7, django-contact-form |release| does not, because the Python core team's
+   support windows for Python 3.6 and 3.7 have ended.
 
 
 What license is django-contact-form under?
 ----------------------------------------------
 
-django-contact-form is offered under a three-clause BSD-style
-license; this is `an OSI-approved open-source license
-<http://www.opensource.org/licenses/bsd-license.php>`_, and allows you
-a large degree of freedom in modifying and redistributing the
-code. For the full terms, see the file `LICENSE` which came with
-your copy of django-contact-form; if you did not receive a copy of
-this file, you can view it online at
+django-contact-form is offered under a three-clause BSD-style license; this is
+`an OSI-approved open-source license
+<http://www.opensource.org/licenses/bsd-license.php>`_, and allows you a large
+degree of freedom in modifying and redistributing the code. For the full terms,
+see the file `LICENSE` which came with your copy of django-contact-form; if you
+did not receive a copy of this file, you can view it online at
 <https://github.com/ubernostrum/django-contact-form/blob/master/LICENSE>.
 
 
 Why aren't there any default templates I can use?
 -------------------------------------------------
 
-Usable default templates, for an application designed to be widely
-reused, are essentially impossible to produce; variations in site
-design, block structure, etc. cannot be reliably accounted for. As
-such, django-contact-form provides bare-bones (i.e., containing no
-HTML structure whatsoever) templates in its source distribution to
-enable running tests, and otherwise just provides good documentation
-of all required templates and the context made available to them.
+Usable default templates, for an application designed to be widely reused, are
+essentially impossible to produce; variations in site design, block structure,
+etc. cannot be reliably accounted for. As such, django-contact-form provides
+bare-bones (i.e., containing no HTML structure whatsoever) templates in its
+source distribution to enable running tests, and otherwise just provides good
+documentation of all required templates and the context made available to them.
 
 
-Why am I getting a bunch of `BadHeaderError` exceptions?
+Why am I getting a bunch of ``BadHeaderError`` exceptions?
 ----------------------------------------------------------
 
 Most likely, you have an error in your
-:class:`~django_contact_form.forms.ContactForm`
-subclass. Specifically, one or more of
-:attr:`~django_contact_form.forms.ContactForm.from_email`,
+:class:`~django_contact_form.forms.ContactForm` subclass. Specifically, one or
+more of :attr:`~django_contact_form.forms.ContactForm.from_email`,
 :attr:`~django_contact_form.forms.ContactForm.recipient_list` or
-:meth:`~django_contact_form.forms.ContactForm.subject` are returning
-values which contain newlines.
+:meth:`~django_contact_form.forms.ContactForm.subject` are returning values
+which contain newlines.
 
 As a security precaution against `email header injection attacks
-<https://en.wikipedia.org/wiki/Email_injection>`_ (which allow
-spammers and other malicious users to manipulate email and potentially
-cause automated systems to send mail to unintended recipients),
-`Django's email-sending framework does not permit newlines in message
-headers
+<https://en.wikipedia.org/wiki/Email_injection>`_ (which allow spammers and
+other malicious users to manipulate email and potentially cause automated
+systems to send mail to unintended recipients), `Django's email-sending
+framework does not permit newlines in message headers
 <https://docs.djangoproject.com/en/stable/topics/email/#preventing-header-injection>`_.
-:exc:`~django.core.mail.BadHeaderError` is the exception Django raises
-when a newline is detected in a header. By default,
-:meth:`~django_contact_form.forms.ContactForm.subject` will forcibly
-condense the subject to a single line.
+:exc:`~django.core.mail.BadHeaderError` is the exception Django raises when a
+newline is detected in a header. By default,
+:meth:`~django_contact_form.forms.ContactForm.subject` will forcibly condense
+the subject to a single line.
 
-Note that this only applies to the headers of an email message; the
-message body can (and usually does) contain newlines.
+Note that this only applies to the headers of an email message; the message
+body can (and usually does) contain newlines.
 
 
 I found a bug or want to make an improvement!
 ---------------------------------------------
 
-The canonical development repository for django-contact-form is
-online at <https://github.com/ubernostrum/django-contact-form>. Issues
-and pull requests can both be filed there.
-
-If you'd like to contribute to django-contact-form, that's great!
-Just please remember that pull requests should include tests and
-documentation for any changes made, and that following `PEP 8
-<https://www.python.org/dev/peps/pep-0008/>`_ is mandatory. Pull
-requests without documentation won't be merged, and PEP 8 style
-violations or test coverage below 100% are both configured to break
-the build.
+The canonical development repository for django-contact-form is online at
+<https://github.com/ubernostrum/django-contact-form>. Issues and pull requests
+can both be filed there.
+
+If you'd like to contribute to django-contact-form, that's great!  Just please
+remember that pull requests should include tests and documentation for any
+changes made, and that following `PEP 8
+<https://www.python.org/dev/peps/pep-0008/>`_ is mandatory. Pull requests
+without documentation won't be merged, and PEP 8 style violations or test
+coverage below 100% are both configured to break the build.
 
 
 I'm getting errors about "akismet" when trying to run tests?
 ------------------------------------------------------------
 
-The full test suite of django-contact-form exercises all of its
-functionality, including the spam-filtering
-:class:`~django_contact_forms.forms.AkismetContactForm`. That class
-uses `the Wordpress Akismet spam-detection service
-<https://akismet.com/>`_ to perform spam filtering, and so requires
-the Python `akismet` module to communicate with the Akismet service,
-and some additional configuration (in the form of a valid Akismet API
-key and associated URL).
+The full test suite of django-contact-form exercises all of its functionality,
+including the spam-filtering
+:class:`~django_contact_form.forms.AkismetContactForm`. That class uses `the
+Wordpress Akismet spam-detection service <https://akismet.com/>`_ to perform
+spam filtering, and so requires the Python `akismet` module to communicate with
+the Akismet service, and some additional configuration (in the form of a valid
+Akismet API key and associated URL).
 
 By default, the tests for
-:class:`~django_contact_forms.forms.AkismetContactForm` will be
-skipped unless the required configuration (in the form of either a
-pair of Django settings, or a pair of environment variables) is
-detected. However, if you have supplied Akismet configuration but do
-*not* have the Python `akismet` module, you will see test errors from
-attempts to import `akismet`. You can resolve this by running::
+:class:`~django_contact_form.forms.AkismetContactForm` will be skipped unless
+the required configuration (in the form of either a pair of Django settings, or
+a pair of environment variables) is detected. However, if you have supplied
+Akismet configuration but do *not* have the Python `akismet` module, you will
+see test errors from attempts to import `akismet`. You can resolve this by
+running:
 
-    pip install akismet
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
+
+      python -m pip install django-contact-form[akismet]
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m pip install django-contact-form[akismet]
 
 or (if you do not intend to use
-:class:`~django_contact_forms.forms.AkismetContactForm`) by no longer
+:class:`~django_contact_form.forms.AkismetContactForm`) by no longer
 configuring the Django settings/environment variables used by Akismet.
 
-Additionally, if the
-:class:`~django_contact_forms.forms.AkismetContactForm` tests are
-skipped, the default code-coverage report will fail due to the
-relevant code not being exercised during the test run.
+Additionally, if the :class:`~django_contact_form.forms.AkismetContactForm`
+tests are skipped, the default code-coverage report will fail due to the
+relevant code not being exercised during the test run.
```

### Comparing `django-contact-form-2.0.1/docs/index.rst` & `django-contact-form-2.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Basic functionality (collecting a name, email address and message) can
 be achieved out of the box by setting up a few templates and adding
 one line to your site's root URLconf:
 
 .. code-block:: python
 
-    path('contact/', include('django_contact_form.urls')),
+    path("contact/", include("django_contact_form.urls")),
 
 For notes on getting started quickly, and on how to customize
 django-contact-form's behavior, read through the full documentation
 below.
 
 
 .. toctree::
@@ -34,8 +34,8 @@
    views
 
 .. toctree::
    :caption: Other documentation
    :maxdepth: 1
 
    upgrade
-   faq
+   faq
```

### Comparing `django-contact-form-2.0.1/docs/install.rst` & `django-contact-form-2.1/docs/install.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,118 @@
 .. _install:
 
 
-Installation guide
-==================
+Installation and recommended configuration
+==========================================
 
-The |release| release of django-contact-form supports Django 3.2 and
-4.0 on Python 3.7 (Django 3.2 only), 3.8, 3.9, and 3.10. Note that
-Django 3.2's support for Python 3.10 was added in Django 3.2.9, so you
-may experience issues with Python 3.10 and earlier Django 3.2
-versions.
+django-contact-form |release| supports Django 3.2, 4.1, and 4.2 on Python 3.8,
+3.9, 3.10, and 3.11 (Django 4.1 and 4.2 only). Note that Django 3.2's support
+for Python 3.10 was added in Django 3.2.9, so you may experience issues with
+Python 3.10 and earlier Django 3.2 versions.
 
+.. note:: **Django 3.2 and supported Python versions**
 
-Normal installation
--------------------
+   Django 3.2 was released before Python 3.10 had come out, and although it now
+   supports Python 3.10, it did not officially do so until the Django 3.2.9
+   release. You may encounter problems if you try to use Django 3.2.8 or
+   earlier with Python 3.10.
 
-The preferred method of installing django-contact-form is via `pip`,
-the standard Python package-installation tool. If you don't have
-`pip`, instructions are available for `how to obtain and install it
-<https://pip.pypa.io/en/latest/installing.html>`_. If you're using a
-supported version of Python, `pip` should have come bundled with your
-installation of Python.
+   Also, although Django 3.2 continues to officially support Python 3.6 and
+   3.7, django-contact-form |release| does not, because the Python core team's
+   support windows for Python 3.6 and 3.7 have ended.
 
-Once you have `pip`, type::
 
-    pip install django-contact-form
+Installing django-contact-form
+------------------------------
 
-If you plan to use the included spam-filtering contact form class,
-:class:`~contact_form.forms.AkismetContactForm`, you will also need
-`the Python akismet module <https://pypi.org/project/akismet/>`_. You
-can manually install it via `pip install akismet`, or tell
-django-contact-form to install it for you, by running::
+To install django-contact-form, run the following command from a command
+prompt/terminal:
 
-    pip install django-contact-form[akismet]
+.. tab:: macOS/Linux/other Unix
 
-If you don't have a copy of a compatible version of Django, installing
-django-contact-form will also automatically install one for you.
+   .. code-block:: shell
 
+      python -m pip install django-contact-form
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m pip install django-contact-form
+
+If you plan to use the spam-filtering
+:class:`~django_contact_form.forms.AkismetContactForm`, you will also need the
+``akismet`` Python library. You can install this separately, or you can have it
+automatically installed for you alongside django-contact-form, by instead
+running:
+
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
+
+      python -m pip install django-contact-form[akismet]
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m pip install django-contact-form[akismet]
+
+This will use ``pip``, the standard Python package-installation tool. If you
+are using a supported version of Python, your installation of Python should
+have come with ``pip`` bundled. If ``pip`` does not appear to be present, you
+can try running the following from a command prompt/terminal:
+
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
+
+      python -m ensurepip --upgrade
+
+.. tab:: Windows
+
+   .. code-block:: shell
+
+      py -m ensurepip --upgrade
+
+Instructions are also available for `how to obtain and manually install or
+upgrade pip <https://pip.pypa.io/en/latest/installation/>`_.
+
+If you don't already have a supported version of Django installed, using
+``pip`` to install django-contact-form will also install the latest
+supported version of Django.
 
 Installing from a source checkout
 ---------------------------------
 
-If you want to work on django-contact-form, you can obtain a source
-checkout.
+If you want to work on django-contact-form, you can obtain a source checkout.
 
 The development repository for django-contact-form is at
-<https://github.com/ubernostrum/django-contact-form>. If you have `git
-<http://git-scm.com/>`_ installed, you can obtain a copy of the
-repository by typing::
+<https://github.com/ubernostrum/django-contact-form>. If you have git
+installed, you can obtain a copy of the repository by typing:
+
+.. code-block:: shell
+
+   git clone https://github.com/ubernostrum/django-contact-form.git
+
+From there, you can use git commands to check out the specific revision you
+want, and perform an “editable” install (allowing you to change code as you
+work on it) by typing:
+
+.. tab:: macOS/Linux/other Unix
+
+   .. code-block:: shell
 
-    git clone https://github.com/ubernostrum/django-contact-form.git
+      python -m pip install -e .
 
-From there, you can use git commands to check out the specific
-revision you want, and perform an "editable" install (allowing you to
-change code as you work on it) by typing::
+.. tab:: Windows
 
-    pip install -e .
+   .. code-block:: shell
 
+      py -m pip install -e .
 
 Next steps
 ----------
 
 To get up and running quickly, check out :ref:`the quick start guide
 <quickstart>`. For full documentation, see :ref:`the documentation
-index <index>`.
+index <index>`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-contact-form-2.0.1/docs/make.bat` & `django-contact-form-2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/docs/quickstart.rst` & `django-contact-form-2.1/docs/quickstart.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,195 +1,183 @@
 .. _quickstart:
 
 Quick start guide
 =================
 
-First you'll need to have Django and django-contact-form
-installed; for details on that, see :ref:`the installation guide
-<install>`.
-
-Once that's done, you can start setting up django-contact-form. First,
-add `'django_contact_form'` to your
-:data:`~django.conf.settings.INSTALLED_APPS` setting. Then, you can
-begin configuring.
+First you'll need to have Django and django-contact-form installed; for details
+on that, see :ref:`the installation guide <install>`.
+
+Once that's done, you can start setting up django-contact-form. Add
+``"django_contact_form"`` to your :setting:`INSTALLED_APPS` setting. Then, you
+can begin configuring.
 
 
 URL configuration
 -----------------
 
-The quickest way to set up the views in django-contact-form is to use
-the provided URLconf, found at `django_contact_form.urls`. You can
-include it wherever you like in your site's URL configuration; for
-example, to have it live at the URL `/contact/`:
+The quickest way to set up the views in django-contact-form is to use the
+provided URLconf, found at ``django_contact_form.urls``. You can include it
+wherever you like in your site's URL configuration; for example, to have it
+live at the URL ``/contact/``:
 
 .. code-block:: python
 
     from django.urls import include, path
 
 
     urlpatterns = [
         # ... other URL patterns for your site ...
-        path('contact/', include('django_contact_form.urls')),
+        path("contact/", include("django_contact_form.urls")),
     ]
 
-If you'll be using a custom form class, you'll need to manually set up
-your URLs so you can tell django-contact-form about your form
-class. For example:
+If you'll be using a custom form class, you'll need to manually set up your
+URLs so you can tell django-contact-form about your form class. For example:
 
 
 .. code-block:: python
 
     from django.urls import include, path
     from django.views.generic import TemplateView
 
     from django_contact_form.views import ContactFormView
 
     from yourapp.forms import YourCustomFormClass
 
 
     urlpatterns = [
         # ... other URL patterns for your site ...
-        path('contact/',
+        path("contact/",
             ContactFormView.as_view(
                 form_class=YourCustomFormClass
             ),
-            name='django_contact_form'),
-        path('contact/sent/',
+            name="django_contact_form"),
+        path("contact/sent/",
             TemplateView.as_view(
-                template_name='django_contact_form/contact_form_sent.html'
+                template_name="django_contact_form/contact_form_sent.html"
             ),
-            name='django_contact_form_sent'),
+            name="django_contact_form_sent"),
     ]
 
 .. important:: **Where to put custom forms and views**
 
    When writing a custom form class (or custom
-   :class:`~django_contact_form.views.ContactFormView` subclass), **don't**
-   put your custom code inside django-contact-form. Instead, put your
-   custom code in the appropriate place (a `forms.py` or `views.py`
-   file) in an application you've written.
+   :class:`~django_contact_form.views.ContactFormView` subclass), **don't** put
+   your custom code inside django-contact-form. Instead, put your custom code
+   in the appropriate place (a ``forms.py`` or ``views.py`` file) in an
+   application you've written.
 
 
 Required templates
 ------------------
 
 The two views above will need several templates to be created.
 
 
-`django_contact_form/contact_form.html`
-```````````````````````````````````````
+``django_contact_form/contact_form.html``
+`````````````````````````````````````````
 
- This is used to display the contact form. It has a
- :class:`~django.template.RequestContext` (so any context processors
- will be applied), and also provides the form instance as the context
- variable `form`.
+This is used to display the contact form. It has a
+:class:`~django.template.RequestContext` (so any context processors will be
+applied), and also provides the form instance as the context variable ``form``.
 
-`django_contact_form/contact_form_sent.html`
-````````````````````````````````````````````
+``django_contact_form/contact_form_sent.html``
+``````````````````````````````````````````````
 
-This is used after a successful form submission, to let the user know
-their message has been sent. It has a
-:class:`~django.template.RequestContext`, but provides no additional
-context variables of its own.
+This is used after a successful form submission, to let the user know their
+message has been sent. It has a :class:`~django.template.RequestContext`, but
+provides no additional context variables of its own.
 
 
-`django_contact_form/contact_form.txt`
-``````````````````````````````````````
+``django_contact_form/contact_form.txt``
+````````````````````````````````````````
 
 Used to render the subject of the email. Will receive a
 :class:`~django.template.RequestContext` with the following additional
 variables:
 
-`body`
-    The message the user typed.
+``body``
+    The message the user supplied.
 
-`email`
+``email``
     The email address the user supplied.
 
-`name`
+``name``
     The name the user supplied.
 
-`site`
-    The current site. Either a
-    :class:`~django.contrib.sites.models.Site` or
-    :class:`~django.contrib.sites.requests.RequestSite` instance,
-    depending on whether `Django's sites framework
+``site``
+    The current site. Either a :class:`~django.contrib.sites.models.Site` or
+    :class:`~django.contrib.sites.requests.RequestSite` instance, depending on
+    whether `Django's sites framework
     <https://docs.djangoproject.com/en/1.11/ref/contrib/sites/>`_ is
     installed).
 
 
-`django_contact_form/contact_form_subject.txt`
-``````````````````````````````````````````````
+``django_contact_form/contact_form_subject.txt``
+````````````````````````````````````````````````
 
 Used to render the subject of the email. Will receive a
 :class:`~django.template.RequestContext` with the following additional
 variables:
 
-`body`
-    The message the user typed.
+``body``
+    The message the user supplied.
 
-`email`
+``email``
     The email address the user supplied.
 
-`name`
+``name``
     The name the user supplied.
 
-`site`
-    The current site. Either a
-    :class:`~django.contrib.sites.models.Site` or
-    :class:`~django.contrib.sites.requests.RequestSite` instance,
-    depending on whether `Django's sites framework
+``site``
+    The current site. Either a :class:`~django.contrib.sites.models.Site` or
+    :class:`~django.contrib.sites.requests.RequestSite` instance, depending on
+    whether `Django's sites framework
     <https://docs.djangoproject.com/en/1.11/ref/contrib/sites/>`_ is
     installed).
 
-.. warning:: **Subject must be a single line**
+    .. warning:: **Subject must be a single line**
 
-   In order to prevent `header injection attacks
-   <https://en.wikipedia.org/wiki/Email_injection>`_, the subject
-   *must* be only a single line of text, and Django's email framework
-   will reject any attempt to send an email with a multi-line
-   subject. So it's a good idea to ensure your
-   `contact_form_subject.txt` template only produces a single line of
-   output when rendered; as a precaution, however, django-contact-form
-   will, by default, condense the output of this template to a single
-   line.
+      In order to prevent `header injection attacks
+      <https://en.wikipedia.org/wiki/Email_injection>`_, the subject *must* be
+      only a single line of text, and Django's email framework will reject any
+      attempt to send an email with a multi-line subject. So it's a good idea
+      to ensure your ``contact_form_subject.txt`` template only produces a
+      single line of output when rendered; as a precaution, however,
+      django-contact-form will, by default, condense the output of this
+      template to a single line.
 
 
 Using a spam-filtering contact form
 -----------------------------------
 
-Spam filtering is a common desire for contact forms, due to the large
-amount of spam they can attract. There is a spam-filtering contact
-form class included in django-contact-form:
-:class:`~django_contact_form.forms.AkismetContactForm`, which uses
-`the Wordpress Akismet spam-detection service
+Spam filtering is a common desire for contact forms, due to the large amount of
+spam they can attract. There is a spam-filtering contact form class included in
+django-contact-form: :class:`~django_contact_form.forms.AkismetContactForm`,
+which uses `the Wordpress Akismet spam-detection service
 <https://akismet.com/>`_.
 
 To use this form, you will need to do the following things:
 
-1. Install the Python `akismet` module to allow django-contact-form
-   to communicate with the Akismet service. You can do this via `pip
-   install akismet`, or as you install django-contact-form via `pip
-   install django-contact-form[akismet]`.
-
-2. Obtain an Akismet API key from <https://akismet.com/>, and
-   associate it with the URL of your site.
-
-3. Supply the API key and URL for django-contact-form to use. You can
-   either place them in the Django settings
-   :data:`~django.conf.settings.AKISMET_API_KEY` and
-   :data:`~django.conf.settings.AKISMET_BLOG_URL`, or in the
-   environment variables `PYTHON_AKISMET_API_KEY` and
-   `PYTHON_AKISMET_BLOG_URL`.
+1. Install the Python ``akismet`` module to allow django-contact-form to
+   communicate with the Akismet service. You can do this via ``pip install
+   akismet``, or as you install django-contact-form via ``pip install
+   django-contact-form[akismet]``.
+
+2. Obtain an Akismet API key from <https://akismet.com/>, and associate it with
+   the URL of your site.
+
+3. Supply the API key and URL for django-contact-form to use. You can either
+   place them in the Django settings :setting:`AKISMET_API_KEY` and
+   :setting:`AKISMET_BLOG_URL`, or in the environment variables
+   ``PYTHON_AKISMET_API_KEY`` and ``PYTHON_AKISMET_BLOG_URL``.
 
 Then you can replace the suggested URLconf above with the following:
 
 .. code-block:: python
 
     from django.urls import include, path
 
 
     urlpatterns = [
         # ... other URL patterns for your site ...
-        path('contact/', include('django_contact_form.akismet_urls')),
+        path("contact/", include("django_contact_form.akismet_urls")),
     ]
-
```

### Comparing `django-contact-form-2.0.1/docs/upgrade.rst` & `django-contact-form-2.1/docs/upgrade.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 .. _upgrade:
 
 Upgrading from previous versions
 ================================
 
-The current release series of django-contact-form is the 2.x series,
-which is not backwards-compatible with the django-contact-form 1.x
-release series.
+The current release series of django-contact-form is the 2.x series, which is
+not backwards-compatible with the django-contact-form 1.x release series.
 
 
 Changes between django-contact-form 1.x and 2.x
 -----------------------------------------------
 
-
 Module renaming
 ~~~~~~~~~~~~~~~
 
 Prior to 2.x, django-contact-form installed a Python module named
-`contact_form`. To avoid silent incompatibilities, and to conform to
-more recent best practices, django-contact-form 2.x now installs a
-module named `django_contact_form`. Attempts to import from the
-`contact_form` module will immediately fail with :exc:`ImportError`.
+``contact_form``. To avoid silent incompatibilities, and to conform to more
+recent best practices, django-contact-form 2.x now installs a module named
+``django_contact_form``. Attempts to import from the ``contact_form`` module
+will immediately fail with :exc:`ImportError`.
 
 Many installations will be able to adapt by replacing references to
-`contact_form` with references to `django_contact_form`.
+``contact_form`` with references to ``django_contact_form``.
 
 
 Template directory renamed
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Similar to the module renaming above, the name of the default
-directory in which django-contact-form looks for templates has changed
-from `contact_form/` to `django_contact_form/`.
-
+Similar to the module renaming above, the name of the default directory in
+which django-contact-form looks for templates has changed from
+``contact_form/`` to ``django_contact_form/``.
 
 .. _renamed-get-context:
 
-Method renamed: get_context() -> get_message_context()
-``````````````````````````````````````````````````````
+Method renamed: ``get_context()`` -> ``get_message_context()``
+``````````````````````````````````````````````````````````````
 
-Prior to 2.x, :class:`~django_contact_form.forms.ContactForm` provided
-a method named `get_context()` which was used to generate the template
-context from which the message would be rendered. However, Django 4.0
-introduced `a new template-based system for rendering forms
+Prior to 2.x, :class:`~django_contact_form.forms.ContactForm` provided a method
+named `get_context()` which was used to generate the template context from
+which the message would be rendered. However, Django 4.0 introduced `a new
+template-based system for rendering forms
 <https://docs.djangoproject.com/en/stable/releases/4.0/#template-based-form-rendering>`_,
 and as a result :class:`django.forms.Form` now has a method named
 :meth:`~django.forms.Form.get_context`.
 
-To resolve this conflict with Django's own base form class, the method
-in django-contact-form has been renamed to
-:meth:`~django_contact_form.forms.ContactForm.get_message_context`,
-which hopefully will not be adopted by any future version of Django's
-own forms system.
-
-If you were previously overriding `get_context()`, you should rename
-your overridden method to
-:meth:`~django_contact_form.forms.ContactForm.get_message_context` to
-ensure it is still called properly. If you have other code which
-called `get_context()`, you should update any such references to call
-:meth:`~django_contact_form.forms.ContactForm.get_message_context`
-instead.
+To resolve this conflict with Django's own base form class, the method in
+django-contact-form has been renamed to
+:meth:`~django_contact_form.forms.ContactForm.get_message_context`, which
+hopefully will not be adopted by any future version of Django's own forms
+system.
+
+If you were previously overriding ``get_context()``, you should rename your
+overridden method to
+:meth:`~django_contact_form.forms.ContactForm.get_message_context` to ensure it
+is still called properly. If you have other code which called
+``get_context()``, you should update any such references to call
+:meth:`~django_contact_form.forms.ContactForm.get_message_context` instead.
```

### Comparing `django-contact-form-2.0.1/runtests.py` & `django-contact-form-2.1/tests/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,45 @@
 """
-A standalone test runner script, configuring the minimum settings
-required for tests to execute.
-
-Re-use at your own risk: many Django applications will require full
-settings and/or templates in order to execute their tests.
+Minimal Django settings file for test runs.
 
 """
-
-import os
-import sys
+import pathlib
 
 from django.utils.crypto import get_random_string
 
-APP_DIR = os.path.abspath(os.path.dirname(__file__))
-
-
-# Minimum settings required for django-contact-form to work.
-SETTINGS_DICT = {
-    "BASE_DIR": APP_DIR,
-    "INSTALLED_APPS": (
-        "django_contact_form",
-        "django.contrib.auth",
-        "django.contrib.contenttypes",
-        "django.contrib.sites",
-    ),
-    "ROOT_URLCONF": "django_contact_form.urls",
-    "DATABASES": {
-        "default": {
-            "ENGINE": "django.db.backends.sqlite3",
-            "NAME": os.path.join(APP_DIR, "db.sqlite3"),
-        }
-    },
-    "MIDDLEWARE": (
-        "django.middleware.common.CommonMiddleware",
-        "django.middleware.csrf.CsrfViewMiddleware",
-    ),
-    "SITE_ID": 1,
-    "DEFAULT_FROM_EMAIL": "contact@example.com",
-    "MANAGERS": [("Manager", "noreply@example.com")],
-    "SECRET_KEY": get_random_string(12),
-    "TEMPLATES": [
-        {
-            "BACKEND": "django.template.backends.django.DjangoTemplates",
-            "DIRS": [os.path.join(APP_DIR, "tests/templates")],
-            "OPTIONS": {
-                "context_processors": [
-                    "django.contrib.auth.context_processors.auth",
-                    "django.template.context_processors.debug",
-                    "django.template.context_processors.i18n",
-                    "django.template.context_processors.media",
-                    "django.template.context_processors.static",
-                    "django.template.context_processors.tz",
-                    "django.contrib.messages.context_processors.messages",
-                ]
-            },
-        }
-    ],
-}
-
-
-def run_tests():
-    # Making Django run this way is a two-step process. First, call
-    # settings.configure() to give Django settings to work with:
-    from django.conf import settings
-
-    settings.configure(**SETTINGS_DICT)
-
-    # Then, call django.setup() to initialize the application cache
-    # and other bits:
-    import django
-
-    django.setup()
-
-    # Now we instantiate a test runner...
-    from django.test.utils import get_runner
-
-    TestRunner = get_runner(settings)
-
-    # And then we run tests and return the results.
-    test_runner = TestRunner(verbosity=2, interactive=True)
-    failures = test_runner.run_tests(["tests"])
-    sys.exit(bool(failures))
-
+APP_DIR = pathlib.Path(__file__).parents[0]
 
-if __name__ == "__main__":
-    run_tests()
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+DEFAULT_FROM_EMAIL = "noreply@example.com"
+DATABASES = {"default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}}
+INSTALLED_APPS = (
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sites",
+    "django_contact_form",
+    "tests",
+)
+MANAGERS = [("Manager", "noreply@example.com")]
+MIDDLEWARE = (
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+)
+ROOT_URLCONF = "django_contact_form.urls"
+SECRET_KEY = get_random_string(12)
+SITE_ID = 1
+TEMPLATES = [
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [APP_DIR / "templates"],
+        "OPTIONS": {
+            "context_processors": [
+                "django.contrib.auth.context_processors.auth",
+                "django.template.context_processors.debug",
+                "django.template.context_processors.i18n",
+                "django.template.context_processors.media",
+                "django.template.context_processors.static",
+                "django.template.context_processors.tz",
+                "django.contrib.messages.context_processors.messages",
+            ]
+        },
+    }
+]
```

### Comparing `django-contact-form-2.0.1/src/django_contact_form/akismet_urls.py` & `django-contact-form-2.1/src/django_contact_form/akismet_urls.py`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo` & `django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po` & `django-contact-form-2.1/src/django_contact_form/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form/urls.py` & `django-contact-form-2.1/src/django_contact_form/urls.py`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/src/django_contact_form.egg-info/PKG-INFO` & `django-contact-form-2.1/src/django_contact_form.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: django-contact-form
-Version: 2.0.1
+Version: 2.1
 Summary: A generic contact-form application for Django
-Home-page: https://github.com/ubernostrum/django-contact-form/
-Author: James Bennett
-Author-email: james@b-list.org
+Author-email: James Bennett <james@b-list.org>
+License: BSD-3-Clause
+Project-URL: documentation, https://django-contact-form.readthedocs.io/
+Project-URL: homepage, https://github.com/ubernostrum/django-contact-form
 Keywords: django,email,contact-form
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: akismet
+Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
 
 .. -*-restructuredtext-*-
 
 .. image:: https://github.com/ubernostrum/django-contact-form/workflows/CI/badge.svg
    :alt: CI status image
    :target: https://github.com/ubernostrum/django-contact-form/actions?query=workflow%3ACI
```

### Comparing `django-contact-form-2.0.1/src/django_contact_form.egg-info/SOURCES.txt` & `django-contact-form-2.1/src/django_contact_form.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+.editorconfig
+.flake8
+.pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
+noxfile.py
+pyproject.toml
 runtests.py
-setup.cfg
-setup.py
-tox.ini
 docs/Makefile
 docs/conf.py
+docs/docs_settings.py
 docs/faq.rst
 docs/forms.rst
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/quickstart.rst
 docs/spelling_wordlist.txt
@@ -20,15 +24,14 @@
 src/django_contact_form/akismet_urls.py
 src/django_contact_form/forms.py
 src/django_contact_form/urls.py
 src/django_contact_form/views.py
 src/django_contact_form.egg-info/PKG-INFO
 src/django_contact_form.egg-info/SOURCES.txt
 src/django_contact_form.egg-info/dependency_links.txt
-src/django_contact_form.egg-info/not-zip-safe
 src/django_contact_form.egg-info/requires.txt
 src/django_contact_form.egg-info/top_level.txt
 src/django_contact_form/locale/da/LC_MESSAGES/django.po
 src/django_contact_form/locale/de/LC_MESSAGES/django.mo
 src/django_contact_form/locale/de/LC_MESSAGES/django.po
 src/django_contact_form/locale/en/LC_MESSAGES/django.mo
 src/django_contact_form/locale/en/LC_MESSAGES/django.po
@@ -40,14 +43,15 @@
 src/django_contact_form/locale/fr/LC_MESSAGES/django.po
 src/django_contact_form/locale/it/LC_MESSAGES/django.po
 src/django_contact_form/locale/nl/LC_MESSAGES/django.mo
 src/django_contact_form/locale/nl/LC_MESSAGES/django.po
 src/django_contact_form/locale/uk/LC_MESSAGES/django.mo
 src/django_contact_form/locale/uk/LC_MESSAGES/django.po
 tests/__init__.py
+tests/settings.py
 tests/test_forms.py
 tests/test_urls.py
 tests/test_views.py
 tests/templates/django_contact_form/contact_form.html
 tests/templates/django_contact_form/contact_form.txt
 tests/templates/django_contact_form/contact_form_sent.html
 tests/templates/django_contact_form/contact_form_subject.txt
```

### Comparing `django-contact-form-2.0.1/tests/test_forms.py` & `django-contact-form-2.1/tests/test_forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Tests for the built-in form classes.
+
+"""
+
 import os
 import unittest
 from unittest import mock
 
 from django.conf import settings
 from django.core import mail
 from django.test import RequestFactory, TestCase
@@ -14,14 +19,18 @@
     Tests the base ContactForm.
 
     """
 
     valid_data = {"name": "Test", "email": "test@example.com", "body": "Test message"}
 
     def request(self):
+        """
+        Construct and return an HttpRequest object for test use.
+
+        """
         return RequestFactory().request()
 
     def test_request_required(self):
         """
         Can't instantiate without an HttpRequest.
 
         """
@@ -88,15 +97,25 @@
         """
         When a template_name() method is defined, it is used and
         preferred over a 'template_name' attribute.
 
         """
 
         class CallableTemplateName(ContactForm):
+            """
+            Form with a template_name() method instead of a template_name attribute.
+
+            """
+
+            # pylint: disable=invalid-overridden-method
             def template_name(self):
+                """
+                Return the template name as a method rather than an attribute.
+
+                """
                 return "django_contact_form/test_callable_template_name.html"
 
         form = CallableTemplateName(request=self.request(), data=self.valid_data)
         self.assertTrue(form.is_valid())
 
         form.save()
         self.assertEqual(1, len(mail.outbox))
@@ -114,24 +133,45 @@
             "from_email": "override@example.com",
             "message": "Overridden message.",
             "recipient_list": ["override_recpt@example.com"],
             "subject": "Overridden subject",
         }
 
         class CallableMessageParts(ContactForm):
+            """
+            Form with the message parts as methods rather than attributes.
+
+            """
+
             def from_email(self):
+                """
+                Method returning the from_email.
+
+                """
                 return overridden_data["from_email"]
 
             def message(self):
+                """
+                Method returning the message.
+
+                """
                 return overridden_data["message"]
 
-            def recipient_list(self):
+            def recipient_list(self):  # pylint: disable=method-hidden
+                """
+                Method returning the recipient_list.
+
+                """
                 return overridden_data["recipient_list"]
 
             def subject(self):
+                """
+                Method returning the subject.
+
+                """
                 return overridden_data["subject"]
 
         form = CallableMessageParts(request=self.request(), data=self.valid_data)
         self.assertTrue(form.is_valid())
 
         self.assertEqual(overridden_data, form.get_message_dict())
 
@@ -144,14 +184,18 @@
 class AkismetContactFormTests(TestCase):
     """
     Tests the Akismet contact form.
 
     """
 
     def request(self):
+        """
+        Construct and return an HttpRequest object for test use.
+
+        """
         return RequestFactory().request()
 
     def test_akismet_form_spam(self):
         """
         The Akismet contact form correctly rejects spam.
 
         """
```

### Comparing `django-contact-form-2.0.1/tests/test_urls.py` & `django-contact-form-2.1/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-contact-form-2.0.1/tests/test_views.py` & `django-contact-form-2.1/tests/test_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Tests for the built-in views.
+
+"""
+
 import os
 import unittest
 from unittest import mock
 
 from django.conf import settings
 from django.core import mail
 from django.test import RequestFactory, TestCase
@@ -9,14 +14,19 @@
 from django.urls import reverse
 
 from django_contact_form.forms import ContactForm
 
 
 @override_settings(ROOT_URLCONF="tests.test_urls")
 class ContactFormViewTests(TestCase):
+    """
+    Tests for the built-in ContactFormView.
+
+    """
+
     def test_get(self):
         """
         HTTP GET on the form view just shows the form.
 
         """
         contact_url = reverse("django_contact_form")
 
@@ -104,14 +114,18 @@
             instance.comment_check.return_value = True
             response = self.client.post(contact_url, data=data)
             self.assertEqual(200, response.status_code)
             self.assertFalse(response.context["form"].is_valid())
             self.assertTrue(response.context["form"].has_error("body"))
 
     def test_akismet_view_ham(self):
+        """
+        The Akismet contact form does not error on non-spam.
+
+        """
         contact_url = reverse("django_contact_form")
         data = {"name": "Test", "email": "email@example.com", "body": "Test message."}
         with mock.patch("akismet.Akismet", autospec=True) as akismet_mock:
             instance = akismet_mock.return_value
             instance.verify_key.return_value = True
             instance.comment_check.return_value = False
             response = self.client.post(contact_url, data=data)
```

