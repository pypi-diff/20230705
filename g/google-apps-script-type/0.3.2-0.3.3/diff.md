# Comparing `tmp/google-apps-script-type-0.3.2.tar.gz` & `tmp/google-apps-script-type-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-apps-script-type-0.3.2.tar", last modified: Mon Jun  5 13:59:59 2023, max compression
+gzip compressed data, was "google-apps-script-type-0.3.3.tar", last modified: Wed Jul  5 15:49:37 2023, max compression
```

## Comparing `google-apps-script-type-0.3.2.tar` & `google-apps-script-type-0.3.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4609 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3695 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/apps/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.667038 google-apps-script-type-0.3.2/google/apps/script/
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/
--rw-rw-r--   0 root         (0)     1003     1262 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/
--rw-rw-r--   0 root         (0)     1003      949 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/__init__.py
--rw-rw-r--   0 root         (0)     1003      253 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/
--rw-rw-r--   0 root         (0)     1003      820 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6251 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/calendar_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/
--rw-rw-r--   0 root         (0)     1003      862 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/__init__.py
--rw-rw-r--   0 root         (0)     1003      245 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.671038 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/
--rw-rw-r--   0 root         (0)     1003      737 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2221 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/docs/types/docs_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/
--rw-rw-r--   0 root         (0)     1003      868 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/__init__.py
--rw-rw-r--   0 root         (0)     1003      247 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/
--rw-rw-r--   0 root         (0)     1003      742 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2325 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/drive/types/drive_addon_manifest.py
--rw-rw-r--   0 root         (0)     1003      235 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/
--rw-rw-r--   0 root         (0)     1003     1017 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/__init__.py
--rw-rw-r--   0 root         (0)     1003      247 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       90 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/
--rw-rw-r--   0 root         (0)     1003      891 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8184 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/gmail_addon_manifest.py
--rw-rw-r--   0 root         (0)     1003       84 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/
--rw-rw-r--   0 root         (0)     1003      874 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/__init__.py
--rw-rw-r--   0 root         (0)     1003      249 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/
--rw-rw-r--   0 root         (0)     1003      747 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2243 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/sheets_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.675038 google-apps-script-type-0.3.2/google/apps/script/type/slides/
--rw-rw-r--   0 root         (0)     1003      874 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/__init__.py
--rw-rw-r--   0 root         (0)     1003      249 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/slides/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/
--rw-rw-r--   0 root         (0)     1003      747 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2243 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/slides/types/slides_addon_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google/apps/script/type/types/
--rw-rw-r--   0 root         (0)     1003     1130 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2417 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/addon_widget_set.py
--rw-rw-r--   0 root         (0)     1003     4023 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/extension_point.py
--rw-rw-r--   0 root         (0)     1003     6314 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/google/apps/script/type/types/script_manifest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/
--rw-r--r--   0 root         (0)     1003     4609 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3401 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-06-05 13:59:59.000000 google-apps-script-type-0.3.2/google_apps_script_type.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2956 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/__init__.py
--rw-rw-r--   0 root         (0)     1003      813 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/calendar/test_calendar.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/docs/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/docs/__init__.py
--rw-rw-r--   0 root         (0)     1003      797 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/docs/test_docs.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.679038 google-apps-script-type-0.3.2/tests/unit/gapic/drive/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/drive/__init__.py
--rw-rw-r--   0 root         (0)     1003      801 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/drive/test_drive.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/__init__.py
--rw-rw-r--   0 root         (0)     1003      801 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/gmail/test_gmail.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/__init__.py
--rw-rw-r--   0 root         (0)     1003      805 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/sheets/test_sheets.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/slides/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/slides/__init__.py
--rw-rw-r--   0 root         (0)     1003      805 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/slides/test_slides.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-06-05 13:59:59.683038 google-apps-script-type-0.3.2/tests/unit/gapic/type/
--rw-rw-r--   0 root         (0)     1003      600 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/type/__init__.py
--rw-rw-r--   0 root         (0)     1003      789 2023-06-05 13:56:51.000000 google-apps-script-type-0.3.2/tests/unit/gapic/type/test_type.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4609 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3695 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.870794 google-apps-script-type-0.3.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.870794 google-apps-script-type-0.3.3/google/apps/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.870794 google-apps-script-type-0.3.3/google/apps/script/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/
+-rw-rw-r--   0 root         (0)     1003     1262 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/calendar/
+-rw-rw-r--   0 root         (0)     1003      949 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/__init__.py
+-rw-rw-r--   0 root         (0)     1003      253 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/calendar/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/calendar/types/
+-rw-rw-r--   0 root         (0)     1003      820 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6251 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/calendar/types/calendar_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/docs/
+-rw-rw-r--   0 root         (0)     1003      862 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/__init__.py
+-rw-rw-r--   0 root         (0)     1003      245 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/docs/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.874795 google-apps-script-type-0.3.3/google/apps/script/type/docs/types/
+-rw-rw-r--   0 root         (0)     1003      737 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2221 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/docs/types/docs_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/drive/
+-rw-rw-r--   0 root         (0)     1003      868 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/__init__.py
+-rw-rw-r--   0 root         (0)     1003      247 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/drive/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/drive/types/
+-rw-rw-r--   0 root         (0)     1003      742 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2325 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/drive/types/drive_addon_manifest.py
+-rw-rw-r--   0 root         (0)     1003      235 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/gmail/
+-rw-rw-r--   0 root         (0)     1003     1017 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/__init__.py
+-rw-rw-r--   0 root         (0)     1003      247 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       90 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/gmail/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/gmail/types/
+-rw-rw-r--   0 root         (0)     1003      891 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8184 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/gmail/types/gmail_addon_manifest.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/sheets/
+-rw-rw-r--   0 root         (0)     1003      874 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      249 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/sheets/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.878795 google-apps-script-type-0.3.3/google/apps/script/type/sheets/types/
+-rw-rw-r--   0 root         (0)     1003      747 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2243 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/sheets/types/sheets_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/google/apps/script/type/slides/
+-rw-rw-r--   0 root         (0)     1003      874 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/__init__.py
+-rw-rw-r--   0 root         (0)     1003      249 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/google/apps/script/type/slides/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/google/apps/script/type/slides/types/
+-rw-rw-r--   0 root         (0)     1003      747 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2243 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/slides/types/slides_addon_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/google/apps/script/type/types/
+-rw-rw-r--   0 root         (0)     1003     1130 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2417 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/types/addon_widget_set.py
+-rw-rw-r--   0 root         (0)     1003     4023 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/types/extension_point.py
+-rw-rw-r--   0 root         (0)     1003     6314 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/google/apps/script/type/types/script_manifest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/
+-rw-r--r--   0 root         (0)     1003     4609 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3401 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:49:37.000000 google-apps-script-type-0.3.3/google_apps_script_type.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2956 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.882796 google-apps-script-type-0.3.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/calendar/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/calendar/__init__.py
+-rw-rw-r--   0 root         (0)     1003      813 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/calendar/test_calendar.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/docs/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/docs/__init__.py
+-rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/docs/test_docs.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/drive/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/drive/__init__.py
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/drive/test_drive.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/gmail/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/gmail/__init__.py
+-rw-rw-r--   0 root         (0)     1003      801 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/gmail/test_gmail.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/sheets/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/sheets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      805 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/sheets/test_sheets.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/slides/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/slides/__init__.py
+-rw-rw-r--   0 root         (0)     1003      805 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/slides/test_slides.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:37.886796 google-apps-script-type-0.3.3/tests/unit/gapic/type/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/type/__init__.py
+-rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-apps-script-type-0.3.3/tests/unit/gapic/type/test_type.py
```

### Comparing `google-apps-script-type-0.3.2/LICENSE` & `google-apps-script-type-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/MANIFEST.in` & `google-apps-script-type-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/PKG-INFO` & `google-apps-script-type-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-script-type
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Apps Script Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-script-type-0.3.2/README.rst` & `google-apps-script-type-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/calendar/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/calendar/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/calendar/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/calendar/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/calendar/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/calendar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/calendar/types/calendar_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/calendar/types/calendar_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/docs/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/docs/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/docs/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/docs/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/docs/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/docs/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/docs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/docs/types/docs_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/docs/types/docs_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/drive/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/drive/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/drive/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/drive/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/drive/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/drive/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/drive/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/drive/types/drive_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/drive/types/drive_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gmail/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gmail/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gmail/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gmail/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gmail/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gmail/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/gmail/types/gmail_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/gmail/types/gmail_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/sheets/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/sheets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/sheets/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/sheets/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/sheets/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/sheets/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/sheets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/sheets/types/sheets_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/sheets/types/sheets_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/slides/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/slides/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/slides/gapic_version.py` & `google-apps-script-type-0.3.3/google/apps/script/type/slides/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.3.2"  # {x-release-please-version}
+__version__ = "0.3.3"  # {x-release-please-version}
```

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/slides/services/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/slides/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/slides/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/slides/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/slides/types/slides_addon_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/slides/types/slides_addon_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/types/__init__.py` & `google-apps-script-type-0.3.3/google/apps/script/type/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/types/addon_widget_set.py` & `google-apps-script-type-0.3.3/google/apps/script/type/types/addon_widget_set.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/types/extension_point.py` & `google-apps-script-type-0.3.3/google/apps/script/type/types/extension_point.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google/apps/script/type/types/script_manifest.py` & `google-apps-script-type-0.3.3/google/apps/script/type/types/script_manifest.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/google_apps_script_type.egg-info/PKG-INFO` & `google-apps-script-type-0.3.3/google_apps_script_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-apps-script-type
-Version: 0.3.2
+Version: 0.3.3
 Summary: Google Apps Script Type API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-apps-script-type-0.3.2/google_apps_script_type.egg-info/SOURCES.txt` & `google-apps-script-type-0.3.3/google_apps_script_type.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/setup.py` & `google-apps-script-type-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/__init__.py` & `google-apps-script-type-0.3.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/calendar/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/calendar/test_calendar.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/calendar/test_calendar.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/docs/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/docs/test_docs.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/docs/test_docs.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/drive/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/drive/test_drive.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/drive/test_drive.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/gmail/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/gmail/test_gmail.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/gmail/test_gmail.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/sheets/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/sheets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/sheets/test_sheets.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/sheets/test_sheets.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/slides/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/slides/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/slides/test_slides.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/slides/test_slides.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/type/__init__.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/type/__init__.py`

 * *Files identical despite different names*

### Comparing `google-apps-script-type-0.3.2/tests/unit/gapic/type/test_type.py` & `google-apps-script-type-0.3.3/tests/unit/gapic/type/test_type.py`

 * *Files identical despite different names*

