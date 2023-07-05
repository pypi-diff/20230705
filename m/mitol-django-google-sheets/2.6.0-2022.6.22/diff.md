# Comparing `tmp/mitol-django-google-sheets-2.6.0.tar.gz` & `tmp/mitol-django-google-sheets-2022.6.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitol-django-google-sheets-2.6.0.tar", last modified: Tue Jan 17 16:20:22 2023, max compression
+gzip compressed data, was "mitol-django-google-sheets-2022.6.22.tar", last modified: Wed Jul  5 16:16:56 2023, max compression
```

## Comparing `mitol-django-google-sheets-2.6.0.tar` & `mitol-django-google-sheets-2022.6.22.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.189221 mitol-django-google-sheets-2.6.0/mitol/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/mitol/google_sheets/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    10412 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12297 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.189221 mitol-django-google-sheets-2.6.0/mitol/google_sheets/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/mitol/google_sheets/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/mitol/google_sheets/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3788 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/migrations/0002_alter_filewatchrenewalattempt_sheet_type.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3139 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/mitol/google_sheets/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/settings/google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (122)    14639 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/sheet_handler_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    15715 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/mitol/google_sheets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 16:20:22.000000 mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-17 16:20:22.193220 mitol-django-google-sheets-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    12013 2023-01-17 16:20:21.000000 mitol-django-google-sheets-2.6.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    10870 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      748 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.983322 mitol-django-google-sheets-2022.6.22/mitol/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       56 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.983322 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      347 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/CHANGELOG.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    10352 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/README.md
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      171 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1916 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/admin.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    12297 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/api.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      405 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/apps.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1071 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/constants.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      958 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/exceptions.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      449 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/factories.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.979988 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/management/
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.983322 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/management/commands/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/management/commands/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/migrations/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3788 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/migrations/0001_initial.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      418 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/migrations/0002_alter_filewatchrenewalattempt_sheet_type.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/migrations/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3139 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/models.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/py.typed
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/settings/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2693 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/settings/google_sheets.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    14639 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/sheet_handler_api.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      450 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/urls.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    15715 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/utils.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2939 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/mitol/google_sheets/views.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    10870 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1140 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      178 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        6 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-07-05 16:16:56.000000 mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/zip-safe
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-07-05 16:16:56.986655 mitol-django-google-sheets-2022.6.22/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11950 2023-07-05 16:16:55.000000 mitol-django-google-sheets-2022.6.22/setup.py
```

### Comparing `mitol-django-google-sheets-2.6.0/PKG-INFO` & `mitol-django-google-sheets-2022.6.22/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets
-Version: 2.6.0
+Version: 2022.6.22
 Summary: Core library to handle Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-google-sheets
 ---
 
 This is the Open Learning Django Google Sheets core library. The purpose of it is to wrap core functionality around Google Sheets for consumption in more feature specific libraries.
 
@@ -47,23 +47,22 @@
 
 *If it's not obvious, remove the angle brackets (`<>`) for the actual values.*
 
 ```dotenv
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_ID=<Client ID from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_SECRET=<Client secret from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_API_PROJECT_ID=<Project ID from step 2>
+MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME=<Name of the app processing the request>
 MITOL_GOOGLE_SHEETS_ENROLLMENT_CHANGE_SHEET_ID=<Change of enrollment request sheet ID from step 3>
 ```
 
 
 ### Usage
+The usage of this library is only possible in conjusction with `mitol-google-sheets-refunds` or `mitol-google-sheets-deferrals`.
 
-In production, webhooks (also known as "file watches") are set up to make a request
-to your app, so that new changes to spreadsheets can be automatically processed. You can set
-those up locally too, but it's probably easier just to use the management commands.
 
 Here's an example workflow for making a request for refunds:
 
 1. Fill out and submit the spreadsheet request form. This should add a row to the
  first worksheet in the enrollment code request spreadsheet.
 2. Run the management command to process the sheet:
  `./manage.py process_refund_requests -i "<spreadsheet id>"`. This should
@@ -194,15 +193,15 @@
     2. OAuth consent screen ([link](https://console.cloud.google.com/apis/credentials/consent))
        1. Under "Test users" click "add users", add your email address
        2. Click "Edit App"
        3. Add a domain in the "Authorized domains" section. **Hit Enter to add**.
        4. **Click Save at the bottom**
     3. Credentials ([link](https://console.cloud.google.com/apis/credentials))
         1. Click on the name of your web app credential in the OAuth 2.0 Client ID section
-        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/api/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/api/sheets/auth-complete/`
+        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/sheets/auth-complete/`
         1. **Click Save**
 7. Log into xPRO via Django admin using the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/admin/`)
 8. Authenticate/authorize the app
     1. Navigate to the sheets admin page (`/sheets/admin/`) with the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/sheets/admin/`)
     1. Click the Authorize button and go through Google OAuth flow
         - *NOTE: You will hit a warning page after selecting your user. To continue, click "Advanced", then click the "Go to \<url\>" link at bottom*
```

### Comparing `mitol-django-google-sheets-2.6.0/backend_shim.py` & `mitol-django-google-sheets-2022.6.22/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/README.md` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,22 @@
 
 *If it's not obvious, remove the angle brackets (`<>`) for the actual values.*
 
 ```dotenv
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_ID=<Client ID from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_SECRET=<Client secret from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_API_PROJECT_ID=<Project ID from step 2>
+MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME=<Name of the app processing the request>
 MITOL_GOOGLE_SHEETS_ENROLLMENT_CHANGE_SHEET_ID=<Change of enrollment request sheet ID from step 3>
 ```
 
 
 ### Usage
+The usage of this library is only possible in conjusction with `mitol-google-sheets-refunds` or `mitol-google-sheets-deferrals`.
 
-In production, webhooks (also known as "file watches") are set up to make a request
-to your app, so that new changes to spreadsheets can be automatically processed. You can set
-those up locally too, but it's probably easier just to use the management commands.
 
 Here's an example workflow for making a request for refunds:
 
 1. Fill out and submit the spreadsheet request form. This should add a row to the
  first worksheet in the enrollment code request spreadsheet.
 2. Run the management command to process the sheet:
  `./manage.py process_refund_requests -i "<spreadsheet id>"`. This should
@@ -180,15 +179,15 @@
     2. OAuth consent screen ([link](https://console.cloud.google.com/apis/credentials/consent))
        1. Under "Test users" click "add users", add your email address
        2. Click "Edit App"
        3. Add a domain in the "Authorized domains" section. **Hit Enter to add**.
        4. **Click Save at the bottom**
     3. Credentials ([link](https://console.cloud.google.com/apis/credentials))
         1. Click on the name of your web app credential in the OAuth 2.0 Client ID section
-        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/api/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/api/sheets/auth-complete/`
+        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/sheets/auth-complete/`
         1. **Click Save**
 7. Log into xPRO via Django admin using the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/admin/`)
 8. Authenticate/authorize the app
     1. Navigate to the sheets admin page (`/sheets/admin/`) with the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/sheets/admin/`)
     1. Click the Authorize button and go through Google OAuth flow
         - *NOTE: You will hit a warning page after selecting your user. To continue, click "Advanced", then click the "Go to \<url\>" link at bottom*
```

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/admin.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/admin.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/api.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/constants.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/constants.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/exceptions.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/migrations/0001_initial.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/models.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/models.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/settings/google_sheets.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/settings/google_sheets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """google sheets settings """
 import pytz
 
 from mitol.common.envs import get_list_literal, get_string
 
 MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME = get_string(
     name="MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME",
+    default=None,
     description="Name of the app processing the request",
-    required=False,
 )
 MITOL_GOOGLE_SHEETS_GOOGLE_ACCOUNT_EMAIL_DOMAIN = get_string(
     name="MITOL_GOOGLE_SHEETS_GOOGLE_ACCOUNT_EMAIL_DOMAIN",
     description="Email domain of the google service account",
     default="iam.gserviceaccount.com",
     required=False,
 )
```

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/sheet_handler_api.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/sheet_handler_api.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/utils.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/utils.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol/google_sheets/views.py` & `mitol-django-google-sheets-2022.6.22/mitol/google_sheets/views.py`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/PKG-INFO` & `mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mitol-django-google-sheets
-Version: 2.6.0
+Version: 2022.6.22
 Summary: Core library to handle Google Sheets integrations in Django
 License: BSD 3-Clause License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 mitol-django-google-sheets
 ---
 
 This is the Open Learning Django Google Sheets core library. The purpose of it is to wrap core functionality around Google Sheets for consumption in more feature specific libraries.
 
@@ -47,23 +47,22 @@
 
 *If it's not obvious, remove the angle brackets (`<>`) for the actual values.*
 
 ```dotenv
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_ID=<Client ID from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_SECRET=<Client secret from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_API_PROJECT_ID=<Project ID from step 2>
+MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME=<Name of the app processing the request>
 MITOL_GOOGLE_SHEETS_ENROLLMENT_CHANGE_SHEET_ID=<Change of enrollment request sheet ID from step 3>
 ```
 
 
 ### Usage
+The usage of this library is only possible in conjusction with `mitol-google-sheets-refunds` or `mitol-google-sheets-deferrals`.
 
-In production, webhooks (also known as "file watches") are set up to make a request
-to your app, so that new changes to spreadsheets can be automatically processed. You can set
-those up locally too, but it's probably easier just to use the management commands.
 
 Here's an example workflow for making a request for refunds:
 
 1. Fill out and submit the spreadsheet request form. This should add a row to the
  first worksheet in the enrollment code request spreadsheet.
 2. Run the management command to process the sheet:
  `./manage.py process_refund_requests -i "<spreadsheet id>"`. This should
@@ -194,15 +193,15 @@
     2. OAuth consent screen ([link](https://console.cloud.google.com/apis/credentials/consent))
        1. Under "Test users" click "add users", add your email address
        2. Click "Edit App"
        3. Add a domain in the "Authorized domains" section. **Hit Enter to add**.
        4. **Click Save at the bottom**
     3. Credentials ([link](https://console.cloud.google.com/apis/credentials))
         1. Click on the name of your web app credential in the OAuth 2.0 Client ID section
-        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/api/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/api/sheets/auth-complete/`
+        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/sheets/auth-complete/`
         1. **Click Save**
 7. Log into xPRO via Django admin using the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/admin/`)
 8. Authenticate/authorize the app
     1. Navigate to the sheets admin page (`/sheets/admin/`) with the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/sheets/admin/`)
     1. Click the Authorize button and go through Google OAuth flow
         - *NOTE: You will hit a warning page after selecting your user. To continue, click "Advanced", then click the "Go to \<url\>" link at bottom*
```

### Comparing `mitol-django-google-sheets-2.6.0/mitol_django_google_sheets.egg-info/SOURCES.txt` & `mitol-django-google-sheets-2022.6.22/mitol_django_google_sheets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitol-django-google-sheets-2.6.0/setup.py` & `mitol-django-google-sheets-2022.6.22/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'description': 'Core library to handle Google Sheets integrations in Django',
     'install_requires': (
         'django<4.0,>=2.2.12',
         'factory-boy~=3.2',
         'google-api-python-client==1.7.11',
         'google-auth-oauthlib>=0.5.2',
         'google-auth==1.6.3',
-        'mitol-django-common~=2.7.0',
+        'mitol-django-common',
         'pygsheets==2.0.2',
         'pytz>=2020.4',
         'setuptools',
     ),
     'license': 'BSD 3-Clause License',
     'long_description': """mitol-django-google-sheets
 ---
@@ -64,23 +64,22 @@
 
 *If it's not obvious, remove the angle brackets (`<>`) for the actual values.*
 
 ```dotenv
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_ID=<Client ID from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_CLIENT_SECRET=<Client secret from step 1>
 MITOL_GOOGLE_SHEETS_DRIVE_API_PROJECT_ID=<Project ID from step 2>
+MITOL_GOOGLE_SHEETS_PROCESSOR_APP_NAME=<Name of the app processing the request>
 MITOL_GOOGLE_SHEETS_ENROLLMENT_CHANGE_SHEET_ID=<Change of enrollment request sheet ID from step 3>
 ```
 
 
 ### Usage
+The usage of this library is only possible in conjusction with `mitol-google-sheets-refunds` or `mitol-google-sheets-deferrals`.
 
-In production, webhooks (also known as "file watches") are set up to make a request
-to your app, so that new changes to spreadsheets can be automatically processed. You can set
-those up locally too, but it's probably easier just to use the management commands.
 
 Here's an example workflow for making a request for refunds:
 
 1. Fill out and submit the spreadsheet request form. This should add a row to the
  first worksheet in the enrollment code request spreadsheet.
 2. Run the management command to process the sheet:
  `./manage.py process_refund_requests -i "<spreadsheet id>"`. This should
@@ -211,15 +210,15 @@
     2. OAuth consent screen ([link](https://console.cloud.google.com/apis/credentials/consent))
        1. Under "Test users" click "add users", add your email address
        2. Click "Edit App"
        3. Add a domain in the "Authorized domains" section. **Hit Enter to add**.
        4. **Click Save at the bottom**
     3. Credentials ([link](https://console.cloud.google.com/apis/credentials))
         1. Click on the name of your web app credential in the OAuth 2.0 Client ID section
-        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/api/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/api/sheets/auth-complete/`
+        1. In the "Authorized redirect URIs" section, click "Add URI", and enter the ngrok HTTPS URL appended with `/sheets/auth-complete/`, e.g.: `https://12345abc6789.ngrok.io/sheets/auth-complete/`
         1. **Click Save**
 7. Log into xPRO via Django admin using the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/admin/`)
 8. Authenticate/authorize the app
     1. Navigate to the sheets admin page (`/sheets/admin/`) with the ngrok HTTP URL (e.g.: `http://12345abc6789.ngrok.io/sheets/admin/`)
     1. Click the Authorize button and go through Google OAuth flow
         - *NOTE: You will hit a warning page after selecting your user. To continue, click "Advanced", then click the "Go to \<url\>" link at bottom*
     
@@ -251,11 +250,11 @@
     'packages': (
         'mitol',
         'mitol.google_sheets',
         'mitol.google_sheets.management.commands',
         'mitol.google_sheets.migrations',
         'mitol.google_sheets.settings',
     ),
-    'python_requires': '>=3.7',
-    'version': '2.6.0',
+    'python_requires': '>=3.8',
+    'version': '2022.6.22',
     'zip_safe': True,
 })
```

