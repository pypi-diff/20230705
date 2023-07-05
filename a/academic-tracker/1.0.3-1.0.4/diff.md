# Comparing `tmp/academic_tracker-1.0.3.tar.gz` & `tmp/academic_tracker-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\academic_tracker-1.0.3.tar", last modified: Wed Mar 16 16:57:37 2022, max compression
+gzip compressed data, was "academic_tracker-1.0.4.tar", last modified: Wed Jul  5 13:45:36 2023, max compression
```

## Comparing `academic_tracker-1.0.3.tar` & `academic_tracker-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,179 @@
-drwxrwxrwx   0        0        0        0 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/
--rw-rw-rw-   0        0        0      105 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1948 2022-03-09 13:56:39.000000 academic_tracker-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      196 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9805 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7262 2022-03-14 20:55:10.000000 academic_tracker-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/academic_tracker/
--rw-rw-rw-   0        0        0     1485 2022-03-16 16:57:29.000000 academic_tracker-1.0.3/academic_tracker/__init__.py
--rw-rw-rw-   0        0        0    22432 2022-03-11 18:43:57.000000 academic_tracker-1.0.3/academic_tracker/__main__.py
--rw-rw-rw-   0        0        0    39922 2022-03-14 19:56:46.000000 academic_tracker-1.0.3/academic_tracker/athr_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0     9576 2022-03-11 17:42:55.000000 academic_tracker-1.0.3/academic_tracker/athr_srch_modularized.py
--rw-rw-rw-   0        0        0    23759 2022-03-11 17:47:46.000000 academic_tracker-1.0.3/academic_tracker/athr_srch_webio.py
--rw-rw-rw-   0        0        0    12932 2022-03-11 17:51:57.000000 academic_tracker-1.0.3/academic_tracker/citation_parsing.py
--rw-rw-rw-   0        0        0     7934 2022-03-11 18:40:23.000000 academic_tracker-1.0.3/academic_tracker/fileio.py
--rw-rw-rw-   0        0        0    21407 2022-03-16 16:11:40.000000 academic_tracker-1.0.3/academic_tracker/helper_functions.py
--rw-rw-rw-   0        0        0    19019 2022-03-11 18:16:58.000000 academic_tracker-1.0.3/academic_tracker/ref_srch_emails_and_reports.py
--rw-rw-rw-   0        0        0     8534 2022-03-11 18:18:31.000000 academic_tracker-1.0.3/academic_tracker/ref_srch_modularized.py
--rw-rw-rw-   0        0        0    21154 2022-03-11 18:22:01.000000 academic_tracker-1.0.3/academic_tracker/ref_srch_webio.py
--rw-rw-rw-   0        0        0    19810 2022-03-16 16:21:27.000000 academic_tracker-1.0.3/academic_tracker/tracker_schema.py
--rw-rw-rw-   0        0        0    13029 2022-03-16 16:25:16.000000 academic_tracker-1.0.3/academic_tracker/user_input_checking.py
--rw-rw-rw-   0        0        0    13468 2022-03-11 18:28:16.000000 academic_tracker-1.0.3/academic_tracker/webio.py
-drwxrwxrwx   0        0        0        0 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/academic_tracker.egg-info/
--rw-rw-rw-   0        0        0     9805 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-03-16 16:57:36.000000 academic_tracker-1.0.3/academic_tracker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/docs/
--rw-rw-rw-   0        0        0      598 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/Makefile
--rw-rw-rw-   0        0        0      795 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/api.rst
--rw-rw-rw-   0        0        0     6350 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/conf.py
--rw-rw-rw-   0        0        0     9862 2022-03-14 19:04:02.000000 academic_tracker-1.0.3/docs/guide.rst
--rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/index.rst
--rw-rw-rw-   0        0        0    35244 2022-03-15 15:11:47.000000 academic_tracker-1.0.3/docs/jsonschema.rst
--rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/license.rst
--rw-rw-rw-   0        0        0    21003 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/reporting.rst
--rw-rw-rw-   0        0        0       40 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/requirements.txt
--rw-rw-rw-   0        0        0      517 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/todo.rst
--rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/tokenization.rst
--rw-rw-rw-   0        0        0    32057 2022-03-08 11:18:32.000000 academic_tracker-1.0.3/docs/tutorial.rst
--rw-rw-rw-   0        0        0      234 2022-03-09 17:05:57.000000 academic_tracker-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-03-16 16:57:37.000000 academic_tracker-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2413 2022-03-14 18:25:40.000000 academic_tracker-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.625418 academic_tracker-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.525989 academic_tracker-1.0.4/.github/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.558659 academic_tracker-1.0.4/.github/workflows/
+-rw-rw-rw-   0        0        0     1480 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/build.yml
+-rw-rw-rw-   0        0        0     1531 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/build_documentation.yml
+-rw-rw-rw-   0        0        0     1241 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/.github/workflows/codecov.yml
+-rw-rw-rw-   0        0        0      165 2023-07-05 12:15:20.000000 academic_tracker-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0      105 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1037 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/CITATION.cff
+-rw-rw-rw-   0        0        0     1948 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      197 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9823 2023-07-05 13:45:36.624390 academic_tracker-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8759 2023-07-05 12:14:25.000000 academic_tracker-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.345114 academic_tracker-1.0.4/docs/
+-rw-rw-rw-   0        0        0      598 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.526986 academic_tracker-1.0.4/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.527993 academic_tracker-1.0.4/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.377817 academic_tracker-1.0.4/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0      801 2022-09-01 18:37:58.000000 academic_tracker-1.0.4/docs/_build/html/_sources/api.rst.txt
+-rw-rw-rw-   0        0        0     8147 2022-09-14 11:26:26.000000 academic_tracker-1.0.4/docs/_build/html/_sources/guide.rst.txt
+-rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0    35244 2022-03-15 15:11:47.000000 academic_tracker-1.0.4/docs/_build/html/_sources/jsonschema.rst.txt
+-rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/license.rst.txt
+-rw-rw-rw-   0        0        0    21003 2022-06-28 19:30:27.000000 academic_tracker-1.0.4/docs/_build/html/_sources/reporting.rst.txt
+-rw-rw-rw-   0        0        0      517 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/todo.rst.txt
+-rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/_build/html/_sources/tokenization.rst.txt
+-rw-rw-rw-   0        0        0    32448 2022-03-24 20:40:49.000000 academic_tracker-1.0.4/docs/_build/html/_sources/tutorial.rst.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.390800 academic_tracker-1.0.4/docs/_build/html/_static/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.528981 academic_tracker-1.0.4/docs/_build/html/_static/css/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.402422 academic_tracker-1.0.4/docs/_build/html/_static/css/fonts/
+-rw-rw-rw-   0        0        0   444379 2022-09-13 14:59:21.000000 academic_tracker-1.0.4/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0      286 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2022-09-09 08:24:14.000000 academic_tracker-1.0.4/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0      801 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/api.rst
+-rw-rw-rw-   0        0        0     6835 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/conf.py
+-rw-rw-rw-   0        0        0     8147 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/guide.rst
+-rw-rw-rw-   0        0        0      661 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/index.rst
+-rw-rw-rw-   0        0        0    35244 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/jsonschema.rst
+-rw-rw-rw-   0        0        0       59 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/license.rst
+-rwxrwxrwx   0        0        0      787 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/make.bat
+-rw-rw-rw-   0        0        0    21003 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/reporting.rst
+-rw-rw-rw-   0        0        0      295 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/docs/requirements.txt
+-rw-rw-rw-   0        0        0      570 2023-07-05 07:49:44.000000 academic_tracker-1.0.4/docs/todo.rst
+-rw-rw-rw-   0        0        0     3162 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/docs/tokenization.rst
+-rw-rw-rw-   0        0        0    32446 2023-07-05 07:49:44.000000 academic_tracker-1.0.4/docs/tutorial.rst
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.424016 academic_tracker-1.0.4/example_configs/
+-rw-rw-rw-   0        0        0    21920 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_project_and_summary_reports_no_duplicates__full_example.json
+-rw-rw-rw-   0        0        0    22499 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__full_example.json
+-rw-rw-rw-   0        0        0     2512 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports__template.json
+-rw-rw-rw-   0        0        0     2457 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/example_configs/many_projects_and_authors_with_summary_reports_no_duplicates__template.json
+-rw-rw-rw-   0        0        0      252 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:45:36.625418 academic_tracker-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2428 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:31.529978 academic_tracker-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.437295 academic_tracker-1.0.4/src/academic_tracker/
+-rw-rw-rw-   0        0        0     1485 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/__init__.py
+-rw-rw-rw-   0        0        0    23047 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/__main__.py
+-rw-rw-rw-   0        0        0    39919 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    10645 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_modularized.py
+-rw-rw-rw-   0        0        0    23904 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/athr_srch_webio.py
+-rw-rw-rw-   0        0        0    12932 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/citation_parsing.py
+-rw-rw-rw-   0        0        0     7934 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/fileio.py
+-rw-rw-rw-   0        0        0    21407 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/helper_functions.py
+-rw-rw-rw-   0        0        0    19018 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0     9348 2023-07-05 11:57:11.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_modularized.py
+-rw-rw-rw-   0        0        0    21154 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/ref_srch_webio.py
+-rw-rw-rw-   0        0        0    19791 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/tracker_schema.py
+-rw-rw-rw-   0        0        0    13114 2023-07-05 11:57:27.000000 academic_tracker-1.0.4/src/academic_tracker/user_input_checking.py
+-rw-rw-rw-   0        0        0    13468 2023-06-30 15:48:36.000000 academic_tracker-1.0.4/src/academic_tracker/webio.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.454162 academic_tracker-1.0.4/src/academic_tracker.egg-info/
+-rw-rw-rw-   0        0        0     9823 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6564 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      215 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 13:45:31.000000 academic_tracker-1.0.4/src/academic_tracker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.517208 academic_tracker-1.0.4/tests/
+-rw-rw-rw-   0        0        0      264 2022-04-05 15:23:06.000000 academic_tracker-1.0.4/tests/conftest.py
+-rw-rw-rw-   0        0        0    15727 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/fixtures.py
+-rw-rw-rw-   0        0        0       78 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/pytest.ini
+-rw-rw-rw-   0        0        0    26868 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_athr_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    22066 2023-07-05 10:39:45.000000 academic_tracker-1.0.4/tests/test_athr_srch_modularized.py
+-rw-rw-rw-   0        0        0    10030 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_athr_srch_webio_no_internet.py
+-rw-rw-rw-   0        0        0     6832 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_citation_parsing.py
+-rw-rw-rw-   0        0        0    14698 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_fileio.py
+-rw-rw-rw-   0        0        0    18175 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_helper_functions.py
+-rw-rw-rw-   0        0        0    21571 2023-07-05 10:45:07.000000 academic_tracker-1.0.4/tests/test_main.py
+-rw-rw-rw-   0        0        0    13183 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_ref_srch_emails_and_reports.py
+-rw-rw-rw-   0        0        0    13615 2023-07-05 11:58:19.000000 academic_tracker-1.0.4/tests/test_ref_srch_modularized.py
+-rw-rw-rw-   0        0        0    13519 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_ref_srch_webio_no_internet.py
+-rw-rw-rw-   0        0        0    41141 2023-07-05 11:22:09.000000 academic_tracker-1.0.4/tests/test_user_input_checking.py
+-rw-rw-rw-   0        0        0     7179 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/test_webio_no_internet.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:45:36.624390 academic_tracker-1.0.4/tests/testing_files/
+-rw-rw-rw-   0        0        0   248560 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_DOI_query.json
+-rw-rw-rw-   0        0        0   665536 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_grant_query.json
+-rw-rw-rw-   0        0        0     4068 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_pub_dict.json
+-rw-rw-rw-   0        0        0  3516898 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/Crossref_query.json
+-rw-rw-rw-   0        0        0   348524 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_author_search_query.json
+-rw-rw-rw-   0        0        0     4463 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_pub_dict.json
+-rw-rw-rw-   0        0        0    13196 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ORCID_query.json
+-rw-rw-rw-   0        0        0    11995 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.docx
+-rw-rw-rw-   0        0        0       50 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.json
+-rw-rw-rw-   0        0        0       28 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/PMID_reference.txt
+-rw-rw-rw-   0        0        0      158 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors.csv
+-rw-rw-rw-   0        0        0      137 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors_missing_column.csv
+-rw-rw-rw-   0        0        0      148 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/add_authors_missing_value.csv
+-rw-rw-rw-   0        0        0     9873 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_project_emails.json
+-rw-rw-rw-   0        0        0     7675 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/athr_project_emails_tabular.json
+-rw-rw-rw-   0        0        0    19935 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_build_author_loop.txt
+-rw-rw-rw-   0        0        0      758 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_build_loop_template_string.txt
+-rw-rw-rw-   0        0        0    10266 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report.txt
+-rw-rw-rw-   0        0        0    53142 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/athr_srch_summary_report_custom_template.txt
+-rw-rw-rw-   0        0        0    13762 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors.json
+-rw-rw-rw-   0        0        0    79728 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_tabular.json
+-rw-rw-rw-   0        0        0    79858 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/authors_by_project_dict_truncated.json
+-rw-rw-rw-   0        0        0     2927 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/collaborator_emails.json
+-rw-rw-rw-   0        0        0     2721 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/collaborator_emails_tabular.json
+-rw-rw-rw-   0        0        0      520 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config.json
+-rw-rw-rw-   0        0        0    16074 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_tabular.json
+-rw-rw-rw-   0        0        0    16210 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated.json
+-rw-rw-rw-   0        0        0    19318 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_authors_adjusted.json
+-rw-rw-rw-   0        0        0    16141 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noCrossref.json
+-rw-rw-rw-   0        0        0    16081 2023-07-05 08:12:50.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noORCID.json
+-rw-rw-rw-   0        0        0    16143 2023-07-05 11:34:38.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_noPubMed.json
+-rw-rw-rw-   0        0        0    16803 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/config_truncated_ref_srch_summary_report.json
+-rw-rw-rw-   0        0        0   127221 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/emails.json
+-rw-rw-rw-   0        0        0        0 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/empty_file.txt
+-rw-rw-rw-   0        0        0     2854 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/gen_reports_ref_summary_report.txt
+-rw-rw-rw-   0        0        0     8639 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/has_author.xml
+-rw-rw-rw-   0        0        0     8305 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/has_pubmed_grants.xml
+-rw-rw-rw-   0        0        0  1085702 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/medline.txt
+-rw-rw-rw-   0        0        0   221143 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/myncbi_webpages.json
+-rw-rw-rw-   0        0        0    22898 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/no_author.xml
+-rw-rw-rw-   0        0        0    26743 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/nsf_award_page.txt
+-rw-rw-rw-   0        0        0     1261 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/parse_citations_test.txt
+-rw-rw-rw-   0        0        0      521 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/project_report.txt
+-rw-rw-rw-   0        0        0    15412 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pub_with_PMCID.xml
+-rw-rw-rw-   0        0        0   376657 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/publication_dict.json
+-rw-rw-rw-   0        0        0    11488 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/publication_dict_truncated.json
+-rw-rw-rw-   0        0        0    15743 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict.json
+-rw-rw-rw-   0        0        0     1245 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pubs_by_author_dict_truncated.json
+-rw-rw-rw-   0        0        0  1111833 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/pymed_pubs.pkl
+-rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_keys_for_citations.json
+-rw-rw-rw-   0        0        0     1916 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_pub_dict.json
+-rw-rw-rw-   0        0        0   278548 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_Crossref_queries.json
+-rw-rw-rw-   0        0        0    32553 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_PubMed_pubs.json
+-rw-rw-rw-   0        0        0     2993 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_gen_reports_test_pub_dict.json
+-rw-rw-rw-   0        0        0      104 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_keys_for_citations.json
+-rw-rw-rw-   0        0        0     6851 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_publication_dict.json
+-rw-rw-rw-   0        0        0     1198 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_default.txt
+-rw-rw-rw-   0        0        0     4141 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular1.csv
+-rw-rw-rw-   0        0        0     2996 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular2.csv
+-rw-rw-rw-   0        0        0     4209 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular3.csv
+-rw-rw-rw-   0        0        0     6522 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_tabular4.xlsx
+-rw-rw-rw-   0        0        0      739 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_template_string.txt
+-rw-rw-rw-   0        0        0     2239 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test1.txt
+-rw-rw-rw-   0        0        0     1781 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/ref_srch_report_test2.txt
+-rw-rw-rw-   0        0        0    12494 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/reference_test.docx
+-rw-rw-rw-   0        0        0      751 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/reference_test.txt
+-rw-rw-rw-   0        0        0     6272 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_DOIs.json
+-rw-rw-rw-   0        0        0     8720 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_author_query.json
+-rw-rw-rw-   0        0        0    37686 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_pub_dict.json
+-rw-rw-rw-   0        0        0    17630 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_pubs.json
+-rw-rw-rw-   0        0        0   244461 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/scholarly_query.json
+-rw-rw-rw-   0        0        0       27 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_csv.csv
+-rw-rw-rw-   0        0        0    11952 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_docx.docx
+-rw-rw-rw-   0        0        0       14 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/testing_text.txt
+-rw-rw-rw-   0        0        0     1118 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenization_report.txt
+-rw-rw-rw-   0        0        0   182317 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_MEDLINE.json
+-rw-rw-rw-   0        0        0   115779 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations.json
+-rw-rw-rw-   0        0        0    86779 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_duplicates_removed.json
+-rw-rw-rw-   0        0        0     1568 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test.json
+-rw-rw-rw-   0        0        0     2225 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test2.json
+-rw-rw-rw-   0        0        0     1170 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_citations_for_report_test_empty.json
+-rw-rw-rw-   0        0        0    44981 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_myncbi_page1.json
+-rw-rw-rw-   0        0        0    34674 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_nsf_award_page.json
+-rw-rw-rw-   0        0        0     3970 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_parsing_test.json
+-rw-rw-rw-   0        0        0     2659 2022-03-08 11:18:32.000000 academic_tracker-1.0.4/tests/testing_files/tokenized_ref_test.json
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `academic_tracker-1.0.3/LICENSE` & `academic_tracker-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/PKG-INFO` & `academic_tracker-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,205 +1,225 @@
 Metadata-Version: 2.1
 Name: academic_tracker
-Version: 1.0.3
+Version: 1.0.4
 Summary: Find publications on PubMed, Crossref, ORCID, and Google Scholar for given authors or references.
 Home-page: https://github.com/MoseleyBioinformaticsLab/academic_tracker
 Author: Travis Thompson
 Author-email: ptth222@gmail.com
 License: BSD
-Description: Academic Tracker
-        ================
-        
-        .. image:: https://img.shields.io/pypi/v/academic_tracker.svg
-           :target: https://pypi.org/project/academic_tracker
-           :alt: Current library version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/academic_tracker.svg
-           :target: https://pypi.org/project/academic_tracker
-           :alt: Supported Python versions
-        
-        .. image:: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml/badge.svg
-           :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml
-           :alt: Build status
-        
-        .. image:: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker/branch/main/graphs/badge.svg?branch=main
-           :target: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker
-           :alt: Code coverage information
-        
-        .. image:: https://img.shields.io/badge/DOI-10.3390%2Fmetabo11030163-blue.svg
-           :target: https://doi.org/10.3390/metabo11030163
-           :alt: Citation link
-        
-        .. image:: https://img.shields.io/github/stars/MoseleyBioinformaticsLab/academic_tracker.svg?style=social&label=Star
-            :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker
-            :alt: GitHub project
-        
-        |
-        
-        Academic Tracker was created to automate the process of making sure that federally 
-        funded publications get listed on PubMed and that the grant funding source for 
-        them is cited. 
-        
-        Academic Tracker is a command line tool to search PubMed, ORCID, Google Scholar, 
-        and Crossref for publications. The program can either be given a list of authors 
-        to look for publications for, or references/citations to publications themselves. 
-        The program will then will look for publications on the aforementioned sources 
-        and return what relevant information is available from those sources.
-        
-        The primary use case is to give the program a list of authors to find publications 
-        for. From this list of publications it can then be determined which ones need 
-        further action to be in compliance.
-        
-        A secondary use case for finding author's publications is to create a report of 
-        the collaborators they have worked with, and can be done by specifying the creation 
-        of that report in the configuration file. Details on reports are in the `documentation <https://moseleybioinformaticslab.github.io/academic_tracker/reporting.html>`__.
-        
-        The other primary use case is to give the program a list of publication references 
-        to find information for.
-        
-        Links
-        ~~~~~
-        
-           * Academic Tracker @ GitHub_
-           * Academic Tracker @ PyPI_
-           * Documentation @ Pages_
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        The Academic Tracker package runs under Python 3.7+. Use pip_ to install.
-        Starting with Python 3.4, pip_ is included by default. Be sure to use the latest 
-        version of pip as older versions are known to have issues grabbing all dependencies. 
-        Academic Tracker relies on sendmail to send emails, so if you need to use that 
-        feature be sure sendmail is installed and in PATH.
-        
-        
-        Install on Linux, Mac OS X
-        --------------------------
-        
-        .. code:: bash
-        
-           python3 -m pip install academic_tracker
-        
-        
-        Install on Windows
-        ------------------
-        
-        .. code:: bash
-        
-           py -3 -m pip install academic_tracker
-           
-        
-        Upgrade on Linux, Mac OS X
-        --------------------------
-        
-        .. code:: bash
-        
-           python3 -m pip install academic_tracker --upgrade
-           
-        
-        Upgrade on Windows
-        ------------------
-        
-        .. code:: bash
-        
-           py -3 -m pip install academic_tracker --upgrade
-        
-        
-        
-        Quickstart
-        ~~~~~~~~~~
-        Academic Tracker has several commands and options. The simplest most common use 
-        case is simply:
-        
-        .. code:: bash
-            
-            academic_tracker author_search config_file.json
-        
-        Academic Tracker's behavior can be quite complex though, so it is highly encouraged 
-        to read the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_ 
-        and `tutorial <https://moseleybioinformaticslab.github.io/academic_tracker/tutorial.html>`_.
-        
-        
-        Creating The Configuration JSON
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        A configuration JSON file is required to run Academic Tracker, but initially creating 
-        it the first time can be burdensome. Unfortunately, there is no easy solution for 
-        this. It is encouraged to read the configuration JSON section in `jsonschema <https://moseleybioinformaticslab.github.io/academic_tracker/jsonschema.html>`_ 
-        and use the example there to create it initially. The add_authors command can help 
-        with building the Authors section if you already have a csv file with author 
-        information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__.
-        
-        
-        Registering With ORCID
-        ~~~~~~~~~~~~~~~~~~~~~~
-        In order to have this program search ORCID you must register with ORCID and obtain 
-        a key and secret. Details on how to do that are `here <https://info.orcid.org/documentation/integration-guide/registering-a-public-api-client/>`__. 
-        If you do not want to do that then the --no_ORCID option can be used to skip searching 
-        ORCID.
-        
-                  
-        Mac OS Note
-        ~~~~~~~~~~~
-        When you try to run the program on Mac OS you may get an SSL error.
-        
-            certificate verify failed: unable to get local issuer certificate
-            
-        This is due to a change in Mac OS and Python. To fix it go to to your Python 
-        folder in Applications and run the Install Certificates.command shell command 
-        in the /Applications/Python 3.x folder. This should fix the issue.
-        
-        
-        Email Sending Note
-        ~~~~~~~~~~~~~~~~~~
-        Academic Tracker uses sendmail to send emails, so any system it is going to be 
-        used on needs to have sendmail installed and the path in PATH. If you try to 
-        send emails without this the program will display a warning. This can be avoided 
-        by using the --test option though. The --test option blocks email sending. Email 
-        sending can also be avoided by leaving the from_email attribute out of the report 
-        sections of the configuration JSON file.
-        
-        
-        How Authors Are Identified
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~
-        When searching by authors it is necessary to confirm that the author given to 
-        Academic Tracker matches the author returned in the query. In general this matching 
-        is done by matching the first and last names and at least one affiliation given 
-        for the author in the configuration JSON file. Note that affiliations can change 
-        over time as authors move, so they may need many affiliations to accurately match 
-        them to their publications depending on how far back you want to search in time.
-        
-        
-        How Publications Are Matched
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        When searching by publications it is necessary to confirm that the publication 
-        in the given reference matches the publication returned in the query. This is done 
-        by either matching the DOIs, PMIDs, or the title and at least one author. Titles 
-        are fuzzy matched using fuzzywuzzy which is why at least one author must also be 
-        matched. Author's are matched using last name and at least one affiliation.
-        
-        
-        License
-        ~~~~~~~
-        This package is distributed under the BSD `license`.
-        
-        
-        .. _GitHub: https://github.com/MoseleyBioinformaticsLab/academic_tracker
-        .. _Pages: https://moseleybioinformaticslab.github.io/academic_tracker/
-        .. _PyPI: https://pypi.org/project/academic_tracker
-        .. _pip: https://pip.pypa.io
 Keywords: PubMed publications citations Crossref ORCID Google Scholar
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Academic Tracker
+================
+
+.. image:: https://img.shields.io/pypi/v/academic_tracker.svg
+   :target: https://pypi.org/project/academic_tracker
+   :alt: Current library version
+
+.. image:: https://img.shields.io/pypi/pyversions/academic_tracker.svg
+   :target: https://pypi.org/project/academic_tracker
+   :alt: Supported Python versions
+
+.. image:: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml
+   :alt: Build status
+
+.. image:: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker/branch/main/graphs/badge.svg?branch=main
+   :target: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker
+   :alt: Code coverage information
+
+.. image:: https://img.shields.io/badge/DOI-10.1371%2Fjournal.pone.0277834-blue.svg
+   :target: https://doi.org/10.1371/journal.pone.0277834
+   :alt: Citation link
+
+.. image:: https://img.shields.io/github/stars/MoseleyBioinformaticsLab/academic_tracker.svg?style=social&label=Star
+    :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker
+    :alt: GitHub project
+
+|
+
+Academic Tracker was created to automate the process of making sure that federally 
+funded publications get listed on PubMed and that the grant funding source for 
+them is cited. 
+
+Academic Tracker is a command line tool to search PubMed, ORCID, Google Scholar, 
+and Crossref for publications. The program can either be given a list of authors 
+to look for publications for, or references/citations to publications themselves. 
+The program will then will look for publications on the aforementioned sources 
+and return what relevant information is available from those sources.
+
+The primary use case is to give the program a list of authors to find publications 
+for. From this list of publications it can then be determined which ones need 
+further action to be in compliance.
+
+A secondary use case for finding author's publications is to create a report of 
+the collaborators they have worked with, and can be done by specifying the creation 
+of that report in the configuration file. Details on reports are in the `documentation <https://moseleybioinformaticslab.github.io/academic_tracker/reporting.html>`__.
+
+The other primary use case is to give the program a list of publication references 
+to find information for.
+
+Links
+~~~~~
+
+   * Academic Tracker @ GitHub_
+   * Academic Tracker @ PyPI_
+   * Documentation @ Pages_
+
+
+Installation
+~~~~~~~~~~~~
+The Academic Tracker package runs under Python 3.8+. Use pip_ to install.
+Starting with Python 3.4, pip_ is included by default. Be sure to use the latest 
+version of pip as older versions are known to have issues grabbing all dependencies. 
+Academic Tracker relies on sendmail to send emails, so if you need to use that 
+feature be sure sendmail is installed and in PATH.
+
+
+Install on Linux, Mac OS X
+--------------------------
+
+.. code:: bash
+
+   python3 -m pip install academic_tracker
+
+
+Install on Windows
+------------------
+
+.. code:: bash
+
+   py -3 -m pip install academic_tracker
+   
+
+Upgrade on Linux, Mac OS X
+--------------------------
+
+.. code:: bash
+
+   python3 -m pip install academic_tracker --upgrade
+   
+
+Upgrade on Windows
+------------------
+
+.. code:: bash
+
+   py -3 -m pip install academic_tracker --upgrade
+
+
+
+Quickstart
+~~~~~~~~~~
+Academic Tracker has several commands and options. The simplest most common use 
+case is simply:
+
+.. code:: bash
+    
+    academic_tracker author_search config_file.json
+    
+Example config files can be downloaded from the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker>`_ 
+directory of the GitHub_.
+
+Academic Tracker's behavior can be quite complex though, so it is highly encouraged 
+to read the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_ 
+and `tutorial <https://moseleybioinformaticslab.github.io/academic_tracker/tutorial.html>`_.
+
+
+Creating The Configuration JSON
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+A configuration JSON file is required to run Academic Tracker, but initially creating 
+it the first time can be burdensome. Unfortunately, there is no easy solution for 
+this. It is encouraged to read the configuration JSON section in `jsonschema <https://moseleybioinformaticslab.github.io/academic_tracker/jsonschema.html>`_ 
+and use the example there to create it initially. The add_authors command can help 
+with building the Authors section if you already have a csv file with author 
+information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__. 
+There are also examples in the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker/tree/main/example_configs>`__ 
+directory of the GitHub repo. There are also more example in the supplemental 
+material of the paper https://doi.org/10.6084/m9.figshare.19412165.
+
+
+Registering With ORCID
+~~~~~~~~~~~~~~~~~~~~~~
+In order to have this program search ORCID you must register with ORCID and obtain 
+a key and secret. Details on how to do that are `here <https://info.orcid.org/documentation/integration-guide/registering-a-public-api-client/>`__. 
+If you do not want to do that then the --no_ORCID option can be used to skip searching 
+ORCID, or don't include the ORCID_search section in the config file.
+
+          
+Mac OS Note
+~~~~~~~~~~~
+When you try to run the program on Mac OS you may get an SSL error.
+
+    certificate verify failed: unable to get local issuer certificate
+    
+This is due to a change in Mac OS and Python. To fix it go to to your Python 
+folder in Applications and run the Install Certificates.command shell command 
+in the /Applications/Python 3.x folder. This should fix the issue.
+
+
+Email Sending Note
+~~~~~~~~~~~~~~~~~~
+Academic Tracker uses sendmail to send emails, so any system it is going to be 
+used on needs to have sendmail installed and the path in PATH. If you try to 
+send emails without this the program will display a warning. This can be avoided 
+by using the --test option though. The --test option blocks email sending. Email 
+sending can also be avoided by leaving the from_email attribute out of the report 
+sections of the configuration JSON file.
+
+
+How Authors Are Identified
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+When searching by authors it is necessary to confirm that the author given to 
+Academic Tracker matches the author returned in the query. In general this matching 
+is done by matching the first and last names and at least one affiliation given 
+for the author in the configuration JSON file. Note that affiliations can change 
+over time as authors move, so they may need many affiliations to accurately match 
+them to their publications depending on how far back you want to search in time.
+
+
+How Publications Are Matched
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+When searching by publications it is necessary to confirm that the publication 
+in the given reference matches the publication returned in the query. This is done 
+by either matching the DOIs, PMIDs, or the title and at least one author. Titles 
+are fuzzy matched using fuzzywuzzy which is why at least one author must also be 
+matched. Author's are matched using last name and at least one affiliation.
+
+
+Troubleshooting Errors
+~~~~~~~~~~~~~~~~~~~~~~
+If you experience errors when running Academic Tracker the first thing to do is 
+simply try again. Since Academic Tracker is communicating with multiple web sources 
+it is not uncommon for a problem to occur with one of these sources. It might also 
+be a good idea to wait several hours or the next day to try again if there is a communication 
+issue with a particular source. You can also use the various "--no_Source" options 
+for whatever source is causing an error. For example, if Crossref keeps having 504 
+HTTP errors you can run with the --no_Crossref option. If the issue persists across 
+multiple runs then try upgrading Academic Tracker's dependencies with 
+"pip install --upgrade dependency_name". The list of dependencies is in the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_.
+
+
+License
+~~~~~~~
+This package is distributed under the BSD `license <https://moseleybioinformaticslab.github.io/academic_tracker/license.html>`__.
+
+
+.. _GitHub: https://github.com/MoseleyBioinformaticsLab/academic_tracker
+.. _Pages: https://moseleybioinformaticslab.github.io/academic_tracker/
+.. _PyPI: https://pypi.org/project/academic_tracker
+.. _pip: https://pip.pypa.io
```

### Comparing `academic_tracker-1.0.3/README.rst` & `academic_tracker-1.0.4/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -13,16 +13,16 @@
    :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml
    :alt: Build status
 
 .. image:: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker/branch/main/graphs/badge.svg?branch=main
    :target: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker
    :alt: Code coverage information
 
-.. image:: https://img.shields.io/badge/DOI-10.3390%2Fmetabo11030163-blue.svg
-   :target: https://doi.org/10.3390/metabo11030163
+.. image:: https://img.shields.io/badge/DOI-10.1371%2Fjournal.pone.0277834-blue.svg
+   :target: https://doi.org/10.1371/journal.pone.0277834
    :alt: Citation link
 
 .. image:: https://img.shields.io/github/stars/MoseleyBioinformaticsLab/academic_tracker.svg?style=social&label=Star
     :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker
     :alt: GitHub project
 
 |
@@ -54,15 +54,15 @@
    * Academic Tracker @ GitHub_
    * Academic Tracker @ PyPI_
    * Documentation @ Pages_
 
 
 Installation
 ~~~~~~~~~~~~
-The Academic Tracker package runs under Python 3.7+. Use pip_ to install.
+The Academic Tracker package runs under Python 3.8+. Use pip_ to install.
 Starting with Python 3.4, pip_ is included by default. Be sure to use the latest 
 version of pip as older versions are known to have issues grabbing all dependencies. 
 Academic Tracker relies on sendmail to send emails, so if you need to use that 
 feature be sure sendmail is installed and in PATH.
 
 
 Install on Linux, Mac OS X
@@ -102,36 +102,42 @@
 ~~~~~~~~~~
 Academic Tracker has several commands and options. The simplest most common use 
 case is simply:
 
 .. code:: bash
     
     academic_tracker author_search config_file.json
+    
+Example config files can be downloaded from the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker>`_ 
+directory of the GitHub_.
 
 Academic Tracker's behavior can be quite complex though, so it is highly encouraged 
 to read the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_ 
 and `tutorial <https://moseleybioinformaticslab.github.io/academic_tracker/tutorial.html>`_.
 
 
 Creating The Configuration JSON
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 A configuration JSON file is required to run Academic Tracker, but initially creating 
 it the first time can be burdensome. Unfortunately, there is no easy solution for 
 this. It is encouraged to read the configuration JSON section in `jsonschema <https://moseleybioinformaticslab.github.io/academic_tracker/jsonschema.html>`_ 
 and use the example there to create it initially. The add_authors command can help 
 with building the Authors section if you already have a csv file with author 
-information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__.
+information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__. 
+There are also examples in the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker/tree/main/example_configs>`__ 
+directory of the GitHub repo. There are also more example in the supplemental 
+material of the paper https://doi.org/10.6084/m9.figshare.19412165.
 
 
 Registering With ORCID
 ~~~~~~~~~~~~~~~~~~~~~~
 In order to have this program search ORCID you must register with ORCID and obtain 
 a key and secret. Details on how to do that are `here <https://info.orcid.org/documentation/integration-guide/registering-a-public-api-client/>`__. 
 If you do not want to do that then the --no_ORCID option can be used to skip searching 
-ORCID.
+ORCID, or don't include the ORCID_search section in the config file.
 
           
 Mac OS Note
 ~~~~~~~~~~~
 When you try to run the program on Mac OS you may get an SSL error.
 
     certificate verify failed: unable to get local issuer certificate
@@ -166,16 +172,29 @@
 When searching by publications it is necessary to confirm that the publication 
 in the given reference matches the publication returned in the query. This is done 
 by either matching the DOIs, PMIDs, or the title and at least one author. Titles 
 are fuzzy matched using fuzzywuzzy which is why at least one author must also be 
 matched. Author's are matched using last name and at least one affiliation.
 
 
+Troubleshooting Errors
+~~~~~~~~~~~~~~~~~~~~~~
+If you experience errors when running Academic Tracker the first thing to do is 
+simply try again. Since Academic Tracker is communicating with multiple web sources 
+it is not uncommon for a problem to occur with one of these sources. It might also 
+be a good idea to wait several hours or the next day to try again if there is a communication 
+issue with a particular source. You can also use the various "--no_Source" options 
+for whatever source is causing an error. For example, if Crossref keeps having 504 
+HTTP errors you can run with the --no_Crossref option. If the issue persists across 
+multiple runs then try upgrading Academic Tracker's dependencies with 
+"pip install --upgrade dependency_name". The list of dependencies is in the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_.
+
+
 License
 ~~~~~~~
-This package is distributed under the BSD `license`.
+This package is distributed under the BSD `license <https://moseleybioinformaticslab.github.io/academic_tracker/license.html>`__.
 
 
 .. _GitHub: https://github.com/MoseleyBioinformaticsLab/academic_tracker
 .. _Pages: https://moseleybioinformaticslab.github.io/academic_tracker/
 .. _PyPI: https://pypi.org/project/academic_tracker
 .. _pip: https://pip.pypa.io
```

### Comparing `academic_tracker-1.0.3/academic_tracker/__init__.py` & `academic_tracker-1.0.4/src/academic_tracker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 ``helper_functions``
     This module contains functions that help the other modules function. The functions do things such as fuzzy matching, regex searching, and printing.
         
 ``webio``
     This module contains general functions for interfacing with the internet.
 
 """
-__version__ = "1.0.3"
+__version__ = "1.0.4"
```

### Comparing `academic_tracker-1.0.3/academic_tracker/__main__.py` & `academic_tracker-1.0.4/src/academic_tracker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-"""   
+"""
 Usage:
-    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --verbose --silent]
-    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --verbose --silent]
+    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --no_PubMed --verbose --silent]
+    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --no_PubMed --verbose --silent]
     academic_tracker find_ORCID <config_json_file> [--verbose --silent]
     academic_tracker find_Google_Scholar <config_json_file> [--verbose --silent]
     academic_tracker add_authors <config_json_file> <authors_file> [--verbose --silent]
     academic_tracker tokenize_reference <references_file_or_URL> [--MEDLINE_reference --verbose --silent]
     academic_tracker gen_reports_and_emails_auth <config_json_file> <publication_json_file> [--test --verbose --silent]
     academic_tracker gen_reports_and_emails_ref <config_json_file> <references_file_or_URL> <publication_json_file> [--test --prev_pub=<file-path> --MEDLINE_reference --verbose --silent]
     
 Options:
     -h --help                         Show this screen.
-    --version                         Show version.
+    -v --version                      Show version.
     --verbose                         Print hidden error messages.
     --silent                          Do not print anything to the screen.
     --test                            Generate pubs and email texts, but do not send emails.
     --prev_pub=<file-path>            Filepath to json or csv with publication ids to ignore. Enter "ignore" for the <file_path> to not look for previous publications.json files in tracker directories.
     
 Reference Type Options:    
     --PMID_reference                  Indicates that the reference_file is a PMID file and only PubMed info will be returned.
     --MEDLINE_reference               Indicates that the reference_file is a MEDLINE file.
 
 Search Options:
     --no_GoogleScholar                Don't search Google Scholar.
     --no_ORCID                        Don't search ORCID.
     --no_Crossref                     Don't search Crossref.
+    --no_PubMed                       Don't search PubMed.
 """
 
 
 import re
 import os
 import datetime
 import sys
@@ -63,22 +64,24 @@
     global VERBOSE
     VERBOSE = args["--verbose"]
     global SILENT
     SILENT = args["--silent"]
     
     if len(sys.argv) > 1 and sys.argv[1] == "author_search":
         author_search(args["<config_json_file>"], args["--no_ORCID"], 
-                      args["--no_GoogleScholar"], args["--no_Crossref"], 
+                      args["--no_GoogleScholar"], args["--no_Crossref"],
+                      args["--no_PubMed"],
                       args["--test"], args["--prev_pub"])
     elif len(sys.argv) > 1 and sys.argv[1] == "reference_search":
         if args["--PMID_reference"]:
             PMID_reference(args["<config_json_file>"], args["<references_file_or_URL>"], args["--test"])
         else:
             reference_search(args["<config_json_file>"], args["<references_file_or_URL>"], 
                              args["--MEDLINE_reference"], args["--no_Crossref"], 
+                             args["--no_PubMed"],
                              args["--test"], args["--prev_pub"])
     elif len(sys.argv) > 1 and sys.argv[1] == "find_ORCID":
         find_ORCID(args["<config_json_file>"])
     elif len(sys.argv) > 1 and sys.argv[1] == "find_Google_Scholar":
         find_Google_Scholar(args["<config_json_file>"])
     elif len(sys.argv) > 1 and sys.argv[1] == "add_authors":
         add_authors(args["<config_json_file>"], args["<authors_file>"])
@@ -91,72 +94,74 @@
                                    args["<publication_json_file>"], args["--MEDLINE_reference"], 
                                    args["--test"], args["--prev_pub"])
     else:
         print("Unrecognized command")  
         
 
 
-def author_search(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref, test, prev_pub_filepath):
+def author_search(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed, test, prev_pub_filepath):
     """Query sources for publications by author.
     
     Reads in the JSON config file, previous publications JSON file, and checks for errors.
     Then searches PubMed, ORCID, Google Scholar, and Crossref for publications for each author.
     Emails are then created and sent to project leaders or individual authors. Emails and
     publications are saved to file and emails are sent depending on the options entered by the user. 
     See the program docstring for options details.
     
     Args:
         config_json_filepath (str): filepath to the configuration JSON.
         no_ORCID (bool): If True search ORCID else don't. Reduces checking on config JSON if True.
         no_GoogleScholar (bool): if True search Google Scholar else don't. Reduces checking on config JSON if True.
         no_Crossref (bool): If True search Crossref else don't. Reduces checking on config JSON if True.
+        no_PubMed (bool): If True search PubMed else don't. Reduces checking on config JSON if True.
         test (bool): If True save_dir_name is tracker-test instead of tracker- and emails are not sent.
         prev_pub_filepath (str or None): filepath to the publication JSON to read in.
     """
     
-    config_dict = athr_srch_modularized.input_reading_and_checking(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref)
+    config_dict = athr_srch_modularized.input_reading_and_checking(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed)
     
     ## Create an authors_json for each project in the config_dict and update those authors attributes with the project attributes.
     authors_by_project_dict, config_dict = athr_srch_modularized.generate_internal_data_and_check_authors(config_dict)
                 
     ## read in previous publications to ignore
     has_previous_pubs, prev_pubs = fileio.read_previous_publications(prev_pub_filepath)
     if has_previous_pubs:
         user_input_checking.prev_pubs_file_check(prev_pubs)
             
     ## Query sources and build publication_dict.
-    publication_dict, prev_pubs = athr_srch_modularized.build_publication_dict(config_dict, prev_pubs, no_ORCID, no_GoogleScholar, no_Crossref)            
+    publication_dict = athr_srch_modularized.build_publication_dict(config_dict, prev_pubs, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed)            
     
     save_dir_name = athr_srch_modularized.save_and_send_reports_and_emails(authors_by_project_dict, publication_dict, config_dict, test)
     
     ## combine previous and new publications lists and save
     fileio.save_publications_to_file(save_dir_name, publication_dict, prev_pubs)
     
     helper_functions.vprint("Success. Publications, reports, and emails saved in " + save_dir_name)
 
 
 
-def reference_search(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, test, prev_pub_filepath):
+def reference_search(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, no_PubMed, test, prev_pub_filepath):
     """Query PubMed and Crossref for publications matching a reference.
     
     Read in user inputs and check for error, query sources based on inputs, build 
     emails and reports, save emails, reports, and publications.
     
     Args:
         config_json_filepath (str): filepath to the configuration JSON.
         ref_path_or_URL (str): either a filepath to file to tokenize or a URL to tokenize.
         MEDLINE_reference (bool): If True re_path_or_URL is a filepath to a MEDLINE formatted file.
         no_Crossref (bool): If True search Crossref else don't. Reduces checking on config JSON if True.
+        no_PubMed (bool): If True search PubMed else don't. Reduces checking on config JSON if True.
         test (bool): If True save_dir_name is tracker-test instead of tracker- and emails are not sent.
         prev_pub_filepath (str or None): filepath to the publication JSON to read in.
     """
     
-    config_dict, tokenized_citations, has_previous_pubs, prev_pubs = ref_srch_modularized.input_reading_and_checking(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, prev_pub_filepath)       
+    config_dict, tokenized_citations, has_previous_pubs, prev_pubs = ref_srch_modularized.input_reading_and_checking(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, no_PubMed, prev_pub_filepath)       
 
-    publication_dict, tokenized_citations = ref_srch_modularized.build_publication_dict(config_dict, tokenized_citations, no_Crossref)
+    publication_dict, tokenized_citations = ref_srch_modularized.build_publication_dict(config_dict, tokenized_citations, no_Crossref, no_PubMed)
             
     save_dir_name = ref_srch_modularized.save_and_send_reports_and_emails(config_dict, tokenized_citations, publication_dict, prev_pubs, has_previous_pubs, test)
             
     fileio.save_publications_to_file(save_dir_name, publication_dict, {})
     fileio.save_json_to_file(save_dir_name, "tokenized_reference.json", tokenized_citations)
     
     helper_functions.vprint("Success. Publications and reports saved in " + save_dir_name)
@@ -172,15 +177,16 @@
         test (bool): If True save_dir_name is tracker-test instead of tracker- and emails are not sent.
     """
     
     ## read in config file
     config_dict = fileio.load_json(config_json_filepath)
     
     ## Get inputs from config file and check them for errors.
-    user_input_checking.ref_config_file_check(config_dict, True)
+    user_input_checking.ref_config_file_check(config_dict, True, False)
+    user_input_checking.config_report_check(config_dict)
     
     ## Check the DOI file extension and call the correct read in function.
     extension = os.path.splitext(ref_path_or_URL)[1][1:].lower()
     if extension == "docx":
         file_contents = fileio.read_text_from_docx(ref_path_or_URL)
     elif extension == "txt":
         file_contents = fileio.read_text_from_txt(ref_path_or_URL)
@@ -363,14 +369,15 @@
         test (bool): If True save_dir_name is tracker-test instead of tracker- and emails are not sent.
     """
     
     config_dict = fileio.load_json(config_json_filepath)
     
     ## Get inputs from config file and check them for errors.
     user_input_checking.tracker_validate(config_dict, tracker_schema.gen_reports_auth_schema)
+    user_input_checking.config_report_check(config_dict)
     
     ## Create an authors_json for each project in the config_dict and update those authors attributes with the project attributes.
     authors_by_project_dict, config_dict = athr_srch_modularized.generate_internal_data_and_check_authors(config_dict)
     
     ## Read in publications.json
     publication_dict = fileio.load_json(publication_json_filepath)
     user_input_checking.prev_pubs_file_check(publication_dict)
@@ -396,14 +403,15 @@
     """
     
     ## read in config file
     config_dict = fileio.load_json(config_json_filepath)
     
     ## Get inputs from config file and check them for errors.
     user_input_checking.tracker_validate(config_dict, tracker_schema.gen_reports_ref_schema)
+    user_input_checking.config_report_check(config_dict)
     
     if not prev_pub_filepath or prev_pub_filepath.lower() == "ignore":
         prev_pubs = {}
         has_previous_pubs = False
     else:
         prev_pubs = fileio.load_json(prev_pub_filepath)
         has_previous_pubs = True
```

### Comparing `academic_tracker-1.0.3/academic_tracker/athr_srch_emails_and_reports.py` & `academic_tracker-1.0.4/src/academic_tracker/athr_srch_emails_and_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,15 +400,15 @@
         df = pandas.DataFrame(collaborators)
         if sort:
             df = df.sort_values(by=sort)
         df = df.drop_duplicates()
         df = df[column_order]
         
         if file_format == "csv":
-            report = df.to_csv(index=False, sep=separator, line_terminator="\n")
+            report = df.to_csv(index=False, sep=separator, lineterminator="\n")
             fileio.save_string_to_file(save_dir_name, filename, report)
         else:
             ## If the file extension isn't .xlsx then there will be an error, so force it.
             extension = os.path.splitext(filename)[1][1:].lower()
             if not extension == "xlsx":
                 filename += ".xlsx"
             
@@ -627,15 +627,15 @@
         df = pandas.DataFrame(rows)
         if sort:
             df = df.sort_values(by=sort)
         df = df.drop_duplicates()
         df = df[column_order]
         
         if file_format == "csv":
-            report = df.to_csv(index=False, sep=separator, line_terminator="\n")
+            report = df.to_csv(index=False, sep=separator, lineterminator="\n")
             fileio.save_string_to_file(save_dir_name, filename, report)
         else:
             ## If the file extension isn't .xlsx then there will be an error, so force it.
             extension = os.path.splitext(filename)[1][1:].lower()
             if not extension == "xlsx":
                 filename += ".xlsx"
             
@@ -709,15 +709,15 @@
         df = pandas.DataFrame(rows)
         if sort:
             df = df.sort_values(by=sort)
         df = df.drop_duplicates()
         df = df[column_order]
         
         if file_format == "csv":
-            report = df.to_csv(index=False, sep=separator, line_terminator="\n")
+            report = df.to_csv(index=False, sep=separator, lineterminator="\n")
             fileio.save_string_to_file(save_dir_name, filename, report)
         else:
             ## If the file extension isn't .xlsx then there will be an error, so force it.
             extension = os.path.splitext(filename)[1][1:].lower()
             if not extension == "xlsx":
                 filename += ".xlsx"
```

### Comparing `academic_tracker-1.0.3/academic_tracker/athr_srch_modularized.py` & `academic_tracker-1.0.4/src/academic_tracker/athr_srch_modularized.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,40 +6,53 @@
 Modularized pieces of author_search.
 """
 import sys
 import re
 import datetime
 import os
 
+import deepdiff
+
 from . import user_input_checking
 from . import fileio
 from . import helper_functions
 from . import athr_srch_webio
 from . import athr_srch_emails_and_reports
 from . import webio
 
 
-def input_reading_and_checking(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref):
+def input_reading_and_checking(config_json_filepath, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed):
     """Read in inputs from user and do error checking.
     
     Args:
         config_json_filepath (str): filepath to the configuration JSON.
         no_ORCID (bool): If True search ORCID else don't. Reduces checking on config JSON if True.
         no_GoogleScholar (bool): if True search Google Scholar else don't. Reduces checking on config JSON if True.
         no_Crossref (bool): If True search Crossref else don't. Reduces checking on config JSON if True.
+        no_PubMed (bool): If True search PubMed else don't. Reduces checking on config JSON if True.
         
     Returns:
         config_dict (dict): Matches the Configuration file JSON schema.
     """
     
     ## read in config file
     config_dict = fileio.load_json(config_json_filepath)
     
+    if not "ORCID_search" in config_dict:
+        no_ORCID = True
+        
+    if not "Crossref_search" in config_dict:
+        no_Crossref = True
+        
+    if not "PubMed_search" in config_dict:
+        no_PubMed = True
+    
     ## Get inputs from config file and check them for errors.
-    user_input_checking.config_file_check(config_dict, no_ORCID, no_GoogleScholar, no_Crossref)
+    user_input_checking.config_file_check(config_dict, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed)
+    user_input_checking.config_report_check(config_dict)
     
     return config_dict
 
 
 
 
 def generate_internal_data_and_check_authors(config_dict):
@@ -69,67 +82,79 @@
         for author in authors_not_in_projects:
             helper_functions.vprint(author)
             
     return authors_by_project_dict, config_dict
 
 
 
-def build_publication_dict(config_dict, prev_pubs, no_ORCID, no_GoogleScholar, no_Crossref):
+def build_publication_dict(config_dict, prev_pubs, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed):
     """Query PubMed, ORCID, Google Scholar, and Crossref for publications for the authors.
     
     Args:
         config_dict (dict): Matches the Configuration file JSON schema.
         prev_pubs (dict): Matches the publication JSON schema. Used to ignore publications when querying.
         no_ORCID (bool): If True search ORCID else don't.
         no_GoogleScholar (bool): if True search Google Scholar else don't.
         no_Crossref (bool): If True search Crossref else don't.
+        no_PubMed (bool): If True search PubMed else don't.
         
     Returns:
         publication_dict (dict): The dictionary matching the publication JSON schema.
         prev_pubs (dict): Same as input, but updated with the new publications found.
     """
     
     ## Get publications from PubMed 
     helper_functions.vprint("Finding author's publications. This could take a while.")
-    helper_functions.vprint("Searching PubMed.")
-    PubMed_publication_dict = athr_srch_webio.search_PubMed_for_pubs(prev_pubs, config_dict["Authors"], config_dict["PubMed_search"]["PubMed_email"])
-    prev_pubs.update(PubMed_publication_dict)
+    current_pubs = {}
+    if not no_PubMed:
+        helper_functions.vprint("Searching PubMed.")
+        PubMed_publication_dict = athr_srch_webio.search_PubMed_for_pubs(current_pubs, config_dict["Authors"], config_dict["PubMed_search"]["PubMed_email"])
+        current_pubs.update(PubMed_publication_dict)
     if not no_ORCID:
         helper_functions.vprint("Searching ORCID.")
-        ORCID_publication_dict = athr_srch_webio.search_ORCID_for_pubs(prev_pubs, config_dict["ORCID_search"]["ORCID_key"], config_dict["ORCID_search"]["ORCID_secret"], config_dict["Authors"])
-        prev_pubs.update(ORCID_publication_dict)
+        ORCID_publication_dict = athr_srch_webio.search_ORCID_for_pubs(current_pubs, config_dict["ORCID_search"]["ORCID_key"], config_dict["ORCID_search"]["ORCID_secret"], config_dict["Authors"])
+        current_pubs.update(ORCID_publication_dict)
     if not no_GoogleScholar:
         helper_functions.vprint("Searching Google Scholar.")
-        Google_Scholar_publication_dict = athr_srch_webio.search_Google_Scholar_for_pubs(prev_pubs, config_dict["Authors"], config_dict["Crossref_search"]["mailto_email"])
-        prev_pubs.update(Google_Scholar_publication_dict)
+        Google_Scholar_publication_dict = athr_srch_webio.search_Google_Scholar_for_pubs(current_pubs, config_dict["Authors"], config_dict["Crossref_search"]["mailto_email"])
+        current_pubs.update(Google_Scholar_publication_dict)
     if not no_Crossref:
         helper_functions.vprint("Searching Crossref.")
-        Crossref_publication_dict = athr_srch_webio.search_Crossref_for_pubs(prev_pubs, config_dict["Authors"], config_dict["Crossref_search"]["mailto_email"])
-        prev_pubs.update(Crossref_publication_dict)
+        Crossref_publication_dict = athr_srch_webio.search_Crossref_for_pubs(current_pubs, config_dict["Authors"], config_dict["Crossref_search"]["mailto_email"])
+        current_pubs.update(Crossref_publication_dict)
     
-    publication_dict = PubMed_publication_dict
+    publication_dict = {}
+    if not no_PubMed:
+        for key, value in PubMed_publication_dict.items():
+            if not key in publication_dict:
+                publication_dict[key] = value
     if not no_ORCID:
         for key, value in ORCID_publication_dict.items():
             if not key in publication_dict:
                 publication_dict[key] = value
     if not no_GoogleScholar:
         for key, value in Google_Scholar_publication_dict.items():
             if not key in publication_dict:
                 publication_dict[key] = value
     if not no_Crossref:
         for key, value in Crossref_publication_dict.items():
             if not key in publication_dict:
                 publication_dict[key] = value
+    
+    ## Compare current pubs with previous and only keep those that are new or updated.
+    for pub_id, pub_values in prev_pubs.items():
+        if pub_id in publication_dict and not deepdiff.DeepDiff(publication_dict[pub_id], pub_values, ignore_order=True, report_repetition=True):
+            del publication_dict[pub_id]
         
         
     if len(publication_dict) == 0:
         helper_functions.vprint("No new publications found.")
         sys.exit()
         
-    return publication_dict, prev_pubs
+    return publication_dict
 
 
 
 def save_and_send_reports_and_emails(authors_by_project_dict, publication_dict, config_dict, test):
     """Build the summary report and project reports and email them.
     
     Args:
```

### Comparing `academic_tracker-1.0.3/academic_tracker/athr_srch_webio.py` & `academic_tracker-1.0.4/src/academic_tracker/athr_srch_webio.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         publications = pubmed.query(author_attributes["pubmed_name_search"], max_results=500)
         
         ## Unpacking pub from publications appears to be the slowest part of the code.
         ## publications is an iterator that is broken up into batches and there are noticeable slow downs each time a new batch is fetched.
         for pub in publications:
             
             pub_id = DOI_URL + pub.doi if pub.doi else pub.pubmed_id.split("\n")[0]
+            ## Sometimes the publication_date can be None, so just skip it.
+            if not pub.publication_date:
+                continue
             publication_date = int(str(pub.publication_date)[:4])
             
             ## if the publication id is in prev_pubs or publication_dict or the publication date is before the curoff year then skip.
             if publication_date < author_attributes["cutoff_year"] or \
                helper_functions.is_pub_in_publication_dict(pub_id, pub.title, prev_pubs, prev_pubs_titles) or \
                helper_functions.is_pub_in_publication_dict(pub_id, pub.title, publication_dict, titles):
                 continue
```

### Comparing `academic_tracker-1.0.3/academic_tracker/citation_parsing.py` & `academic_tracker-1.0.4/src/academic_tracker/citation_parsing.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/academic_tracker/fileio.py` & `academic_tracker-1.0.4/src/academic_tracker/fileio.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 This module contains the functions that read and write files.
 """
 
 
 import re
 import os
 import sys
+import json
 
 import docx
-import json
 import pandas
 
 from . import helper_functions
 
 
 
 def load_json(filepath):
```

### Comparing `academic_tracker-1.0.3/academic_tracker/helper_functions.py` & `academic_tracker-1.0.4/src/academic_tracker/helper_functions.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/academic_tracker/ref_srch_emails_and_reports.py` & `academic_tracker-1.0.4/src/academic_tracker/ref_srch_emails_and_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         df = pandas.DataFrame(rows)
         if sort:
             df = df.sort_values(by=sort)
         df = df.drop_duplicates()
         df = df[column_order]
         
         if file_format == "csv":
-            report = df.to_csv(index=False, sep=separator, line_terminator="\n")
+            report = df.to_csv(index=False, sep=separator, lineterminator="\n")
             fileio.save_string_to_file(save_dir_name, filename, report)
         else:
             ## If the file extension isn't .xlsx then there will be an error, so force it.
             extension = os.path.splitext(filename)[1][1:].lower()
             if not extension == "xlsx":
                 filename += ".xlsx"
```

### Comparing `academic_tracker-1.0.3/academic_tracker/ref_srch_modularized.py` & `academic_tracker-1.0.4/src/academic_tracker/ref_srch_modularized.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,36 +15,44 @@
 from . import helper_functions
 from . import ref_srch_webio
 from . import ref_srch_emails_and_reports
 from . import webio
 
 
 
-def input_reading_and_checking(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, prev_pub_filepath):
+def input_reading_and_checking(config_json_filepath, ref_path_or_URL, MEDLINE_reference, no_Crossref, no_PubMed, prev_pub_filepath):
     """Read in inputs from user and do error checking.
     
     Args:
         config_json_filepath (str): filepath to the configuration JSON.
         ref_path_or_URL (str): either a filepath to file to tokenize or a URL to tokenize.
         MEDLINE_reference (bool): If True re_path_or_URL is a filepath to a MEDLINE formatted file.
         no_Crossref (bool): If True search Crossref else don't. Reduces checking on config JSON if True.
+        no_PubMed (bool): If True search PubMed else don't. Reduces checking on config JSON if True.
         prev_pub_filepath (str or None): filepath to the publication JSON to read in.
         
     Returns:
         config_dict (dict): Matches the Configuration file JSON schema.
         tokenized_citations (list): list of dicts. Matches the tokenized citations JSON schema.
         has_previous_pubs (bool): True if a prev_pub file was input, False otherwise.
         prev_pubs (dict): The contents of the prev_pub file input by the user if provided.
     """
     
     ## read in config file
     config_dict = fileio.load_json(config_json_filepath)
     
+    if not "Crossref_search" in config_dict:
+        no_Crossref = True
+        
+    if not "PubMed_search" in config_dict:
+        no_PubMed = True
+    
     ## Get inputs from config file and check them for errors.
-    user_input_checking.ref_config_file_check(config_dict, no_Crossref)
+    user_input_checking.ref_config_file_check(config_dict, no_Crossref, no_PubMed)
+    user_input_checking.config_report_check(config_dict)
     
     if not prev_pub_filepath or prev_pub_filepath.lower() == "ignore":
         prev_pubs = {}
         has_previous_pubs = False
     else:
         prev_pubs = fileio.load_json(prev_pub_filepath)
         has_previous_pubs = True
@@ -54,48 +62,56 @@
         
     tokenized_citations = ref_srch_webio.tokenize_reference_input(ref_path_or_URL, MEDLINE_reference) 
     
     return config_dict, tokenized_citations, has_previous_pubs, prev_pubs
 
 
 
-def build_publication_dict(config_dict, tokenized_citations, no_Crossref):
+def build_publication_dict(config_dict, tokenized_citations, no_Crossref, no_PubMed):
     """Query PubMed and Crossref for publications matching the citations in tokenized_citations.
     
     Args:
         config_dict (dict): Matches the Configuration file JSON schema.
         tokenized_citations (list): list of dicts. Matches the tokenized citations JSON schema.
         no_Crossref (bool): If True search Crossref else don't. Reduces checking on config JSON if True.
+        no_PubMed (bool): If True search PubMed else don't. Reduces checking on config JSON if True.
         
     Returns:
         publication_dict (dict): The dictionary matching the publication JSON schema.
         tokenized_citations (list): Same list as the input but with the pud_dict_key updated to match the publication found.        
     """
     
     helper_functions.vprint("Finding publications. This could take a while.")
-    helper_functions.vprint("Searching PubMed.")
-    PubMed_publication_dict, PubMed_matching_key_for_citation = ref_srch_webio.search_references_on_PubMed(tokenized_citations, config_dict["PubMed_search"]["PubMed_email"])
+    if not no_PubMed:
+        helper_functions.vprint("Searching PubMed.")
+        PubMed_publication_dict, PubMed_matching_key_for_citation = ref_srch_webio.search_references_on_PubMed(tokenized_citations, config_dict["PubMed_search"]["PubMed_email"])
 #    if not args["--no_GoogleScholar"]:
 #        print("Searching Google Scholar.")
 #        Google_Scholar_publication_dict, Google_Scholar_matching_key_for_citation = webio.search_references_on_Google_Scholar(tokenized_citations, config_dict["Crossref_search"]["Crossref_email"], args["--verbose"])
     if not no_Crossref:
         helper_functions.vprint("Searching Crossref.")
         Crossref_publication_dict, Crossref_matching_key_for_citation = ref_srch_webio.search_references_on_Crossref(tokenized_citations, config_dict["Crossref_search"]["mailto_email"])
     
-    publication_dict = PubMed_publication_dict
+    publication_dict = {}
+    if not no_PubMed:
+        for key, value in PubMed_publication_dict.items():
+            if not key in publication_dict:
+                publication_dict[key] = value
 #    if not args["--no_GoogleScholar"]:
 #        for key, value in Google_Scholar_publication_dict.items():
 #            if not key in publication_dict:
 #                publication_dict[key] = value
     if not no_Crossref:
         for key, value in Crossref_publication_dict.items():
             if not key in publication_dict:
                 publication_dict[key] = value
             
-    matching_key_for_citation = PubMed_matching_key_for_citation
+    matching_key_for_citation = [None] * len(tokenized_citations)
+    if not no_PubMed:
+        matching_key_for_citation = [key if key else PubMed_matching_key_for_citation[count] for count, key in enumerate(matching_key_for_citation)]
 #    if not args["--no_GoogleScholar"]:
 #        matching_key_for_citation = [key if key else Google_Scholar_matching_key_for_citation[count] for count, key in enumerate(matching_key_for_citation)]
     if not no_Crossref:
         matching_key_for_citation = [key if key else Crossref_matching_key_for_citation[count] for count, key in enumerate(matching_key_for_citation)]
         
     for count, citation in enumerate(tokenized_citations):
         if matching_key_for_citation[count]:
```

### Comparing `academic_tracker-1.0.3/academic_tracker/ref_srch_webio.py` & `academic_tracker-1.0.4/src/academic_tracker/ref_srch_webio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/academic_tracker/tracker_schema.py` & `academic_tracker-1.0.4/src/academic_tracker/tracker_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import copy
 
 ## TODO add the file inputs and look into adding file existence checking in jsonschema format checker.
 cli_schema = {
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "title": "Command Line Inputs",
- "description": "Input file that contains information for how the program should run.",
+ "description": "Schema to check that program arguments are valid.",
  
  "type": "object",
  "properties": {
          "--prev_pub": {"type":["string", "null"], "minLength":1},
          },
          
 }
```

### Comparing `academic_tracker-1.0.3/academic_tracker/user_input_checking.py` & `academic_tracker-1.0.4/src/academic_tracker/user_input_checking.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,116 +123,125 @@
 
 
 
 
 
 
 
-def config_file_check(config_json, no_ORCID, no_GoogleScholar, no_Crossref):
+def config_file_check(config_json, no_ORCID, no_GoogleScholar, no_Crossref, no_PubMed):
     """Check that the configuration JSON file is as expected.
     
     The validational jsonschema is in the tracker_schema module. 
     
     Args:
-        config_json (dict): dict with the same structure as the configuration JSON file
+        config_json (dict): dict with the same structure as the configuration JSON file.
+        no_ORCID (bool): if True delete the part of the schema that checks ORCID attributes.
+        no_GoogleScholar (bool): if True and no_Crossref is True delete the part of the schema that checks Crossref attributes.
+        no_Crossref (bool): if True and no_GoogleScholar is True delete the part of the schema that checks Crossref attributes.
+        no_PubMed (bool): if True delete the part of the schema that checks PubMed attributes.
     """
     
     schema = copy.deepcopy(tracker_schema.config_schema)
     if no_ORCID:
         del schema["properties"]["ORCID_search"]
         schema["required"].remove("ORCID_search")
     if no_Crossref and no_GoogleScholar:
         del schema["properties"]["Crossref_search"]
         schema["required"].remove("Crossref_search")
+    if no_PubMed:
+        del schema["properties"]["PubMed_search"]
+        schema["required"].remove("PubMed_search")
     
     pattern_messages = {"ORCID":" is not a valid ORCID. It must match the regex \d{4}-\d{4}-\d{4}-\d{3}[0,1,2,3,4,5,6,7,8,9,X]"}
     tracker_validate(instance=config_json, schema=schema, pattern_messages=pattern_messages, format_checker=jsonschema.FormatChecker())
-    
-    ## Make sure sort and column_order only have values in columns for any report.
-    attributes_to_check = ["sort", "column_order"]
-    for attribute in attributes_to_check:
-        if "summary_report" in config_json and "columns" in config_json["summary_report"] and attribute in config_json["summary_report"]:
-            names_not_in_columns = [name for name in config_json["summary_report"][attribute] if not name in config_json["summary_report"]["columns"]]
-            if names_not_in_columns:
-                helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the summary_report has values that are not column names in \"columns\".")
-                helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
-                sys.exit()   
-                
-            if attribute == "column_order":
-                if len(config_json["summary_report"]["column_order"]) != len(config_json["summary_report"]["columns"]):
-                    helper_functions.vprint("ValidationError: The \"column_order\" attribute for the summary_report does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
-                    sys.exit() 
-            
-            
-    report_keys = ["collaborator_report", "project_report"]
-    for project, project_attributes in config_json["project_descriptions"].items():
-        for report_key in report_keys:
-            for attribute in attributes_to_check:
-                if report_key in project_attributes and "columns" in project_attributes[report_key] and attribute in project_attributes[report_key]:
-                    names_not_in_columns = [name for name in project_attributes[report_key][attribute] if not name in project_attributes[report_key]["columns"]]
-                    if names_not_in_columns:
-                        helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the " + report_key + " in project " + project + " has values that are not column names in \"columns\".")
-                        helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
-                        sys.exit()
-                        
-                    if attribute == "column_order":
-                        if len(project_attributes[report_key]["column_order"]) != len(project_attributes[report_key]["columns"]):
-                            helper_functions.vprint("ValidationError: The \"column_order\" attribute for the " + report_key + " in project " + project + " does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
-                            sys.exit() 
-                                    
-    
-    for author, author_attributes in config_json["Authors"].items():
-        for report_key in report_keys:
-            for attribute in attributes_to_check:
-                if report_key in author_attributes and "columns" in author_attributes[report_key] and attribute in author_attributes[report_key]:
-                    names_not_in_columns = [name for name in author_attributes[report_key][attribute] if not name in author_attributes[report_key]["columns"]]
-                    if names_not_in_columns:
-                        helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the " + report_key + " for author " + author + " has values that are not column names in \"columns\".")
-                        helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
-                        sys.exit()
-                        
-                    if attribute == "column_order":
-                        if len(author_attributes[report_key]["column_order"]) != len(author_attributes[report_key]["columns"]):
-                            helper_functions.vprint("ValidationError: The \"column_order\" attribute for the " + report_key + " for author " + author + " does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
-                            sys.exit() 
-                    
-        
+
+
             
 
-def ref_config_file_check(config_json, no_Crossref):
+def ref_config_file_check(config_json, no_Crossref, no_PubMed):
     """Check that the configuration JSON file is as expected.
     
     The validational jsonschema is in the tracker_schema module.    
     
     Args:
-        config_json (dict): dict with a truncated structure of the configuration JSON file
+        config_json (dict): dict with a truncated structure of the configuration JSON file.
+        no_Crossref (bool): if True delete the part of the schema that checks Crossref attributes.
+        no_PubMed (bool): if True delete the part of the schema that checks PubMed attributes.
     """
     
     schema = copy.deepcopy(tracker_schema.ref_config_schema)
     if no_Crossref:
         del schema["properties"]["Crossref_search"]
         schema["required"].remove("Crossref_search")
+    if no_PubMed:
+        del schema["properties"]["PubMed_search"]
+        schema["required"].remove("PubMed_search")
     
-    tracker_validate(instance=config_json, schema=schema, format_checker=jsonschema.FormatChecker())
+    tracker_validate(instance=config_json, schema=schema, format_checker=jsonschema.FormatChecker())    
+
 
+
+def config_report_check(config_json):
+    """Check that the report attributes don't have conflicts.
+    
+    Make sure that the values in sort and column_order are in columns, 
+    and that every column is in column_order.
+    
+    Args:
+        config_json (dict): dict with the same structure as the configuration JSON file.
+    """
     ## Make sure sort and column_order only have values in columns for any report.
     attributes_to_check = ["sort", "column_order"]
     for attribute in attributes_to_check:
         if "summary_report" in config_json and "columns" in config_json["summary_report"] and attribute in config_json["summary_report"]:
             names_not_in_columns = [name for name in config_json["summary_report"][attribute] if not name in config_json["summary_report"]["columns"]]
             if names_not_in_columns:
                 helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the summary_report has values that are not column names in \"columns\".")
                 helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
-                sys.exit()    
+                sys.exit()   
                 
             if attribute == "column_order":
                 if len(config_json["summary_report"]["column_order"]) != len(config_json["summary_report"]["columns"]):
                     helper_functions.vprint("ValidationError: The \"column_order\" attribute for the summary_report does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
                     sys.exit() 
-        
+            
+    
+    if "project_descriptions" in config_json:        
+        report_keys = ["collaborator_report", "project_report"]
+        for project, project_attributes in config_json["project_descriptions"].items():
+            for report_key in report_keys:
+                for attribute in attributes_to_check:
+                    if report_key in project_attributes and "columns" in project_attributes[report_key] and attribute in project_attributes[report_key]:
+                        names_not_in_columns = [name for name in project_attributes[report_key][attribute] if not name in project_attributes[report_key]["columns"]]
+                        if names_not_in_columns:
+                            helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the " + report_key + " in project " + project + " has values that are not column names in \"columns\".")
+                            helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
+                            sys.exit()
+                            
+                        if attribute == "column_order":
+                            if len(project_attributes[report_key]["column_order"]) != len(project_attributes[report_key]["columns"]):
+                                helper_functions.vprint("ValidationError: The \"column_order\" attribute for the " + report_key + " in project " + project + " does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
+                                sys.exit() 
+                                    
+    
+    if "Authors" in config_json:
+        for author, author_attributes in config_json["Authors"].items():
+            for report_key in report_keys:
+                for attribute in attributes_to_check:
+                    if report_key in author_attributes and "columns" in author_attributes[report_key] and attribute in author_attributes[report_key]:
+                        names_not_in_columns = [name for name in author_attributes[report_key][attribute] if not name in author_attributes[report_key]["columns"]]
+                        if names_not_in_columns:
+                            helper_functions.vprint("ValidationError: The \"" + attribute + "\" attribute for the " + report_key + " for author " + author + " has values that are not column names in \"columns\".")
+                            helper_functions.vprint("The following names in \"" + attribute + "\" could not be matched to a column in \"columns\":\n\n" + "\n".join(names_not_in_columns))
+                            sys.exit()
+                            
+                        if attribute == "column_order":
+                            if len(author_attributes[report_key]["column_order"]) != len(author_attributes[report_key]["columns"]):
+                                helper_functions.vprint("ValidationError: The \"column_order\" attribute for the " + report_key + " for author " + author + " does not have all of the column names in \"columns\". Every column in \"columns\" must be in \"column_order\".")
+                                sys.exit()     
 
 
 
 def prev_pubs_file_check(prev_pubs):
     """Run input checking on prev_pubs dict.
     
     The validational jsonschema is in the tracker_schema module.
```

### Comparing `academic_tracker-1.0.3/academic_tracker/webio.py` & `academic_tracker-1.0.4/src/academic_tracker/webio.py`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/academic_tracker.egg-info/PKG-INFO` & `academic_tracker-1.0.4/src/academic_tracker.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,205 +1,225 @@
 Metadata-Version: 2.1
 Name: academic-tracker
-Version: 1.0.3
+Version: 1.0.4
 Summary: Find publications on PubMed, Crossref, ORCID, and Google Scholar for given authors or references.
 Home-page: https://github.com/MoseleyBioinformaticsLab/academic_tracker
 Author: Travis Thompson
 Author-email: ptth222@gmail.com
 License: BSD
-Description: Academic Tracker
-        ================
-        
-        .. image:: https://img.shields.io/pypi/v/academic_tracker.svg
-           :target: https://pypi.org/project/academic_tracker
-           :alt: Current library version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/academic_tracker.svg
-           :target: https://pypi.org/project/academic_tracker
-           :alt: Supported Python versions
-        
-        .. image:: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml/badge.svg
-           :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml
-           :alt: Build status
-        
-        .. image:: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker/branch/main/graphs/badge.svg?branch=main
-           :target: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker
-           :alt: Code coverage information
-        
-        .. image:: https://img.shields.io/badge/DOI-10.3390%2Fmetabo11030163-blue.svg
-           :target: https://doi.org/10.3390/metabo11030163
-           :alt: Citation link
-        
-        .. image:: https://img.shields.io/github/stars/MoseleyBioinformaticsLab/academic_tracker.svg?style=social&label=Star
-            :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker
-            :alt: GitHub project
-        
-        |
-        
-        Academic Tracker was created to automate the process of making sure that federally 
-        funded publications get listed on PubMed and that the grant funding source for 
-        them is cited. 
-        
-        Academic Tracker is a command line tool to search PubMed, ORCID, Google Scholar, 
-        and Crossref for publications. The program can either be given a list of authors 
-        to look for publications for, or references/citations to publications themselves. 
-        The program will then will look for publications on the aforementioned sources 
-        and return what relevant information is available from those sources.
-        
-        The primary use case is to give the program a list of authors to find publications 
-        for. From this list of publications it can then be determined which ones need 
-        further action to be in compliance.
-        
-        A secondary use case for finding author's publications is to create a report of 
-        the collaborators they have worked with, and can be done by specifying the creation 
-        of that report in the configuration file. Details on reports are in the `documentation <https://moseleybioinformaticslab.github.io/academic_tracker/reporting.html>`__.
-        
-        The other primary use case is to give the program a list of publication references 
-        to find information for.
-        
-        Links
-        ~~~~~
-        
-           * Academic Tracker @ GitHub_
-           * Academic Tracker @ PyPI_
-           * Documentation @ Pages_
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        The Academic Tracker package runs under Python 3.7+. Use pip_ to install.
-        Starting with Python 3.4, pip_ is included by default. Be sure to use the latest 
-        version of pip as older versions are known to have issues grabbing all dependencies. 
-        Academic Tracker relies on sendmail to send emails, so if you need to use that 
-        feature be sure sendmail is installed and in PATH.
-        
-        
-        Install on Linux, Mac OS X
-        --------------------------
-        
-        .. code:: bash
-        
-           python3 -m pip install academic_tracker
-        
-        
-        Install on Windows
-        ------------------
-        
-        .. code:: bash
-        
-           py -3 -m pip install academic_tracker
-           
-        
-        Upgrade on Linux, Mac OS X
-        --------------------------
-        
-        .. code:: bash
-        
-           python3 -m pip install academic_tracker --upgrade
-           
-        
-        Upgrade on Windows
-        ------------------
-        
-        .. code:: bash
-        
-           py -3 -m pip install academic_tracker --upgrade
-        
-        
-        
-        Quickstart
-        ~~~~~~~~~~
-        Academic Tracker has several commands and options. The simplest most common use 
-        case is simply:
-        
-        .. code:: bash
-            
-            academic_tracker author_search config_file.json
-        
-        Academic Tracker's behavior can be quite complex though, so it is highly encouraged 
-        to read the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_ 
-        and `tutorial <https://moseleybioinformaticslab.github.io/academic_tracker/tutorial.html>`_.
-        
-        
-        Creating The Configuration JSON
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        A configuration JSON file is required to run Academic Tracker, but initially creating 
-        it the first time can be burdensome. Unfortunately, there is no easy solution for 
-        this. It is encouraged to read the configuration JSON section in `jsonschema <https://moseleybioinformaticslab.github.io/academic_tracker/jsonschema.html>`_ 
-        and use the example there to create it initially. The add_authors command can help 
-        with building the Authors section if you already have a csv file with author 
-        information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__.
-        
-        
-        Registering With ORCID
-        ~~~~~~~~~~~~~~~~~~~~~~
-        In order to have this program search ORCID you must register with ORCID and obtain 
-        a key and secret. Details on how to do that are `here <https://info.orcid.org/documentation/integration-guide/registering-a-public-api-client/>`__. 
-        If you do not want to do that then the --no_ORCID option can be used to skip searching 
-        ORCID.
-        
-                  
-        Mac OS Note
-        ~~~~~~~~~~~
-        When you try to run the program on Mac OS you may get an SSL error.
-        
-            certificate verify failed: unable to get local issuer certificate
-            
-        This is due to a change in Mac OS and Python. To fix it go to to your Python 
-        folder in Applications and run the Install Certificates.command shell command 
-        in the /Applications/Python 3.x folder. This should fix the issue.
-        
-        
-        Email Sending Note
-        ~~~~~~~~~~~~~~~~~~
-        Academic Tracker uses sendmail to send emails, so any system it is going to be 
-        used on needs to have sendmail installed and the path in PATH. If you try to 
-        send emails without this the program will display a warning. This can be avoided 
-        by using the --test option though. The --test option blocks email sending. Email 
-        sending can also be avoided by leaving the from_email attribute out of the report 
-        sections of the configuration JSON file.
-        
-        
-        How Authors Are Identified
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~
-        When searching by authors it is necessary to confirm that the author given to 
-        Academic Tracker matches the author returned in the query. In general this matching 
-        is done by matching the first and last names and at least one affiliation given 
-        for the author in the configuration JSON file. Note that affiliations can change 
-        over time as authors move, so they may need many affiliations to accurately match 
-        them to their publications depending on how far back you want to search in time.
-        
-        
-        How Publications Are Matched
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        When searching by publications it is necessary to confirm that the publication 
-        in the given reference matches the publication returned in the query. This is done 
-        by either matching the DOIs, PMIDs, or the title and at least one author. Titles 
-        are fuzzy matched using fuzzywuzzy which is why at least one author must also be 
-        matched. Author's are matched using last name and at least one affiliation.
-        
-        
-        License
-        ~~~~~~~
-        This package is distributed under the BSD `license`.
-        
-        
-        .. _GitHub: https://github.com/MoseleyBioinformaticsLab/academic_tracker
-        .. _Pages: https://moseleybioinformaticslab.github.io/academic_tracker/
-        .. _PyPI: https://pypi.org/project/academic_tracker
-        .. _pip: https://pip.pypa.io
 Keywords: PubMed publications citations Crossref ORCID Google Scholar
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Academic Tracker
+================
+
+.. image:: https://img.shields.io/pypi/v/academic_tracker.svg
+   :target: https://pypi.org/project/academic_tracker
+   :alt: Current library version
+
+.. image:: https://img.shields.io/pypi/pyversions/academic_tracker.svg
+   :target: https://pypi.org/project/academic_tracker
+   :alt: Supported Python versions
+
+.. image:: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml/badge.svg
+   :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker/actions/workflows/build.yml
+   :alt: Build status
+
+.. image:: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker/branch/main/graphs/badge.svg?branch=main
+   :target: https://codecov.io/gh/MoseleyBioinformaticsLab/academic_tracker
+   :alt: Code coverage information
+
+.. image:: https://img.shields.io/badge/DOI-10.1371%2Fjournal.pone.0277834-blue.svg
+   :target: https://doi.org/10.1371/journal.pone.0277834
+   :alt: Citation link
+
+.. image:: https://img.shields.io/github/stars/MoseleyBioinformaticsLab/academic_tracker.svg?style=social&label=Star
+    :target: https://github.com/MoseleyBioinformaticsLab/academic_tracker
+    :alt: GitHub project
+
+|
+
+Academic Tracker was created to automate the process of making sure that federally 
+funded publications get listed on PubMed and that the grant funding source for 
+them is cited. 
+
+Academic Tracker is a command line tool to search PubMed, ORCID, Google Scholar, 
+and Crossref for publications. The program can either be given a list of authors 
+to look for publications for, or references/citations to publications themselves. 
+The program will then will look for publications on the aforementioned sources 
+and return what relevant information is available from those sources.
+
+The primary use case is to give the program a list of authors to find publications 
+for. From this list of publications it can then be determined which ones need 
+further action to be in compliance.
+
+A secondary use case for finding author's publications is to create a report of 
+the collaborators they have worked with, and can be done by specifying the creation 
+of that report in the configuration file. Details on reports are in the `documentation <https://moseleybioinformaticslab.github.io/academic_tracker/reporting.html>`__.
+
+The other primary use case is to give the program a list of publication references 
+to find information for.
+
+Links
+~~~~~
+
+   * Academic Tracker @ GitHub_
+   * Academic Tracker @ PyPI_
+   * Documentation @ Pages_
+
+
+Installation
+~~~~~~~~~~~~
+The Academic Tracker package runs under Python 3.8+. Use pip_ to install.
+Starting with Python 3.4, pip_ is included by default. Be sure to use the latest 
+version of pip as older versions are known to have issues grabbing all dependencies. 
+Academic Tracker relies on sendmail to send emails, so if you need to use that 
+feature be sure sendmail is installed and in PATH.
+
+
+Install on Linux, Mac OS X
+--------------------------
+
+.. code:: bash
+
+   python3 -m pip install academic_tracker
+
+
+Install on Windows
+------------------
+
+.. code:: bash
+
+   py -3 -m pip install academic_tracker
+   
+
+Upgrade on Linux, Mac OS X
+--------------------------
+
+.. code:: bash
+
+   python3 -m pip install academic_tracker --upgrade
+   
+
+Upgrade on Windows
+------------------
+
+.. code:: bash
+
+   py -3 -m pip install academic_tracker --upgrade
+
+
+
+Quickstart
+~~~~~~~~~~
+Academic Tracker has several commands and options. The simplest most common use 
+case is simply:
+
+.. code:: bash
+    
+    academic_tracker author_search config_file.json
+    
+Example config files can be downloaded from the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker>`_ 
+directory of the GitHub_.
+
+Academic Tracker's behavior can be quite complex though, so it is highly encouraged 
+to read the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_ 
+and `tutorial <https://moseleybioinformaticslab.github.io/academic_tracker/tutorial.html>`_.
+
+
+Creating The Configuration JSON
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+A configuration JSON file is required to run Academic Tracker, but initially creating 
+it the first time can be burdensome. Unfortunately, there is no easy solution for 
+this. It is encouraged to read the configuration JSON section in `jsonschema <https://moseleybioinformaticslab.github.io/academic_tracker/jsonschema.html>`_ 
+and use the example there to create it initially. The add_authors command can help 
+with building the Authors section if you already have a csv file with author 
+information. A good tool to help track down pesky JSON syntax errors is `here <https://csvjson.com/json_validator>`__. 
+There are also examples in the `example_configs <https://github.com/MoseleyBioinformaticsLab/academic_tracker/tree/main/example_configs>`__ 
+directory of the GitHub repo. There are also more example in the supplemental 
+material of the paper https://doi.org/10.6084/m9.figshare.19412165.
+
+
+Registering With ORCID
+~~~~~~~~~~~~~~~~~~~~~~
+In order to have this program search ORCID you must register with ORCID and obtain 
+a key and secret. Details on how to do that are `here <https://info.orcid.org/documentation/integration-guide/registering-a-public-api-client/>`__. 
+If you do not want to do that then the --no_ORCID option can be used to skip searching 
+ORCID, or don't include the ORCID_search section in the config file.
+
+          
+Mac OS Note
+~~~~~~~~~~~
+When you try to run the program on Mac OS you may get an SSL error.
+
+    certificate verify failed: unable to get local issuer certificate
+    
+This is due to a change in Mac OS and Python. To fix it go to to your Python 
+folder in Applications and run the Install Certificates.command shell command 
+in the /Applications/Python 3.x folder. This should fix the issue.
+
+
+Email Sending Note
+~~~~~~~~~~~~~~~~~~
+Academic Tracker uses sendmail to send emails, so any system it is going to be 
+used on needs to have sendmail installed and the path in PATH. If you try to 
+send emails without this the program will display a warning. This can be avoided 
+by using the --test option though. The --test option blocks email sending. Email 
+sending can also be avoided by leaving the from_email attribute out of the report 
+sections of the configuration JSON file.
+
+
+How Authors Are Identified
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+When searching by authors it is necessary to confirm that the author given to 
+Academic Tracker matches the author returned in the query. In general this matching 
+is done by matching the first and last names and at least one affiliation given 
+for the author in the configuration JSON file. Note that affiliations can change 
+over time as authors move, so they may need many affiliations to accurately match 
+them to their publications depending on how far back you want to search in time.
+
+
+How Publications Are Matched
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+When searching by publications it is necessary to confirm that the publication 
+in the given reference matches the publication returned in the query. This is done 
+by either matching the DOIs, PMIDs, or the title and at least one author. Titles 
+are fuzzy matched using fuzzywuzzy which is why at least one author must also be 
+matched. Author's are matched using last name and at least one affiliation.
+
+
+Troubleshooting Errors
+~~~~~~~~~~~~~~~~~~~~~~
+If you experience errors when running Academic Tracker the first thing to do is 
+simply try again. Since Academic Tracker is communicating with multiple web sources 
+it is not uncommon for a problem to occur with one of these sources. It might also 
+be a good idea to wait several hours or the next day to try again if there is a communication 
+issue with a particular source. You can also use the various "--no_Source" options 
+for whatever source is causing an error. For example, if Crossref keeps having 504 
+HTTP errors you can run with the --no_Crossref option. If the issue persists across 
+multiple runs then try upgrading Academic Tracker's dependencies with 
+"pip install --upgrade dependency_name". The list of dependencies is in the `guide <https://moseleybioinformaticslab.github.io/academic_tracker/guide.html>`_.
+
+
+License
+~~~~~~~
+This package is distributed under the BSD `license <https://moseleybioinformaticslab.github.io/academic_tracker/license.html>`__.
+
+
+.. _GitHub: https://github.com/MoseleyBioinformaticsLab/academic_tracker
+.. _Pages: https://moseleybioinformaticslab.github.io/academic_tracker/
+.. _PyPI: https://pypi.org/project/academic_tracker
+.. _pip: https://pip.pypa.io
```

### Comparing `academic_tracker-1.0.3/docs/Makefile` & `academic_tracker-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/docs/api.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/api.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 API
 ===
 
 .. automodule:: academic_tracker
 
+
 .. automodule:: academic_tracker.user_input_checking
     :members:
 
 .. automodule:: academic_tracker.athr_srch_modularized
     :members:
 .. automodule:: academic_tracker.athr_srch_webio
     :members:
 .. automodule:: academic_tracker.athr_srch_emails_and_reports
     :members:
 
+
 .. automodule:: academic_tracker.ref_srch_modularized
     :members:
 .. automodule:: academic_tracker.ref_srch_webio
     :members:
 .. automodule:: academic_tracker.ref_srch_emails_and_reports
     :members:
+
 .. automodule:: academic_tracker.citation_parsing
     :members:
 
 .. automodule:: academic_tracker.fileio
     :members:
 .. automodule:: academic_tracker.helper_functions
     :members:
```

### Comparing `academic_tracker-1.0.3/docs/conf.py` & `academic_tracker-1.0.4/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 # sys.path.insert(0, os.path.abspath('.'))
-sys.path.insert(0, os.path.abspath('..'))
+sys.path.insert(0, os.path.abspath('../src'))
  
 from academic_tracker import __version__
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Academic Tracker'
@@ -66,15 +66,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -196,7 +196,24 @@
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {'https://docs.python.org/': None}
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
+
+
+
+# def process_main_docstring(app, what, name, obj, options, lines):
+#     if what == 'module' and "__main__" in name:
+#         for i in range(len(lines)):
+#             lines[i] = "   " + lines[i]
+#         lines.insert(0, "")
+#         lines.insert(0, ".. code-block:: console")
+
+# def setup(app):
+#     app.connect('autodoc-process-docstring', process_main_docstring)
+
+
+rinoh_documents = [
+    dict(doc='index', target='AcademicTracker', template='article')
+]
```

### Comparing `academic_tracker-1.0.3/docs/index.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/docs/jsonschema.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/jsonschema.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/docs/reporting.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/reporting.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -297,17 +297,17 @@
     Jerika Durham    Differential Fuel Requirements of Human NK Cells and Human CD8 T Cells: Glutamine Regulates Glucose Uptake in Strongly Activated CD8 T Cells
     Pan Deng         Nutritional modulation of the toxicity of environmental pollutants: Implications in atherosclerosis
     Pan Deng         SSIF: Subsumption-based sub-term inference framework to audit gene ontology
     Pan Deng         MEScan: a powerful statistical framework for genome-scale mutual exclusivity analysis of cancer mutations
 
 
 Default Template Strings
-~~~~~~~~~~~~~~~~~~~~~~~~
+------------------------
 Author Search
--------------
+~~~~~~~~~~~~~
 Summary
 +++++++
 .. code-block:: console
 
     <project_loop><project_name>\n<author_loop>\t<author_first> <author_last>:<pub_loop>\n\t\tTitle: <title> \n\t\tAuthors: <authors> \n\t\tJournal: <journal> \n\t\tDOI: <DOI> \n\t\tPMID: <PMID> \n\t\tPMCID: <PMCID> \n\t\tGrants: <grants>\n</pub_loop>\n</author_loop></project_loop>
```

### Comparing `academic_tracker-1.0.3/docs/todo.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/todo.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/docs/tokenization.rst` & `academic_tracker-1.0.4/docs/_build/html/_sources/tokenization.rst.txt`

 * *Files identical despite different names*

### Comparing `academic_tracker-1.0.3/docs/tutorial.rst` & `academic_tracker-1.0.4/docs/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 Search For Publications By Author
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --verbose --silent]
+    academic_tracker author_search <config_json_file> [--test --prev_pub=<file-path> --no_GoogleScholar --no_ORCID --no_Crossref --no_PubMed --verbose --silent]
 
 
 Description
 -----------
 For each author in the Authors section of the configuration JSON file search 
 PubMed, ORCID, Crossref, and Google Scholar for publications they are an author 
 on. The cutoff_year attribute for either the projects or the authors can be used 
@@ -86,14 +86,19 @@
 
 If used author_search will not search ORCID for publications.
 
 --no_Crossref: 
 
 If used author_search will not search Crossref for publications.
 
+--no_PubMed: 
+
+If used author_search will not search PubMed for publications. This option is 
+assumed if the PubMed_search section of the configuration JSON file is missing.
+
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
 
 --silent:
 
 If used nothing will be printed to the screen.
@@ -352,15 +357,15 @@
 
 Search For Publications By Reference
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Command Line Signature
 ----------------------
 .. code-block:: console
 
-    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --verbose --silent]
+    academic_tracker reference_search <config_json_file> <references_file_or_URL> [--test --prev_pub=<file-path> --PMID_reference --MEDLINE_reference --no_Crossref --no_PubMed --verbose --silent]
 
 
 Description
 -----------
 Parse and tokenize the reference file or URL and then search PubMed and Crossref 
 for the publications found. ORCID is not searched because it is a database of 
 authors and does not support searching for publications directly. Google Scholar 
@@ -419,14 +424,19 @@
 
 Specifies that the reference file is a MEDLINE_ formatted file.
             
 --no_Crossref: 
 
 If used reference_search will not search Crossref for publications.
 
+--no_PubMed: 
+
+If used reference_search will not search Crossref for publications. This option 
+is assumed if the PubMed_search section of the configuration JSON file is missing.
+
 --verbose: 
 
 If used HTML errors and other warnings will be printed to the screen.
 
 --silent:
 
 If used nothing will be printed to the screen.
```

### Comparing `academic_tracker-1.0.3/setup.py` & `academic_tracker-1.0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def readme():
     with open('README.rst') as readme_file:
         return readme_file.read()
 
 
 def find_version():
-    with open('academic_tracker/__init__.py', 'r') as fd:
+    with open('src/academic_tracker/__init__.py', 'r') as fd:
         version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
                             fd.read(), re.MULTILINE).group(1)
     if not version:
         raise RuntimeError('Cannot find version information')
     return version
 
 
@@ -33,44 +33,45 @@
     "jsonschema >= 4.4.0",
     "habanero >= 1.0.0",
     "orcid >= 1.0.3",
     "scholarly >= 1.4.5",
     "beautifulsoup4 >= 4.9.3",
     "fuzzywuzzy >= 0.18.0",
     "python-docx >= 0.8.11",
-    "pandas >= 0.24.2",
+    "pandas >= 1.3.5",
     "openpyxl >= 2.6.2",
     "requests >= 2.21.0",
+    "deepdiff >= 5.7.0"
 ]
 
 
 setup(
     name='academic_tracker',
     version=find_version(),
     author='Travis Thompson',
     author_email='ptth222@gmail.com',
     description='Find publications on PubMed, Crossref, ORCID, and Google Scholar for given authors or references.',
     keywords='PubMed publications citations Crossref ORCID Google Scholar',
     license='BSD',
     url='https://github.com/MoseleyBioinformaticsLab/academic_tracker',
-    packages=find_packages(exclude=['doc', 'docs', 'vignettes']),
+    packages=find_packages("src", exclude=['doc', 'docs', 'vignettes']),
+    package_dir={'': 'src'},
     platforms=['any'],
     long_description=readme(),
     long_description_content_type="text/x-rst",
     install_requires=REQUIRES,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     entry_points={"console_scripts": ["academic_tracker = academic_tracker.__main__:main"]},
 )
```

