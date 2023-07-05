# Comparing `tmp/ora2-5.0.4.tar.gz` & `tmp/ora2-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ora2-5.0.4.tar", last modified: Wed Jul  5 14:20:30 2023, max compression
+gzip compressed data, was "ora2-5.1.0.tar", last modified: Wed Jul  5 14:21:01 2023, max compression
```

## Comparing `ora2-5.0.4.tar` & `ora2-5.1.0.tar`

### file list

```diff
@@ -1,551 +1,558 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.138190 ora2-5.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-07-05 14:20:14.000000 ora2-5.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-05 14:20:14.000000 ora2-5.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-05 14:20:30.138190 ora2-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-05 14:20:14.000000 ora2-5.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.998188 ora2-5.0.4/openassessment/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.998188 ora2-5.0.4/openassessment/assessment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.002188 ora2-5.0.4/openassessment/assessment/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/self.py
--rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/api/teams.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.002188 ora2-5.0.4/openassessment/assessment/errors/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/self.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/errors/student_training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.002188 ora2-5.0.4/openassessment/assessment/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0002_staffworkflow.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0003_expand_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0006_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/0007_staff_workflow_blank.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.006188 ora2-5.0.4/openassessment/assessment/models/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/models/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/score_type_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.006188 ora2-5.0.4/openassessment/assessment/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/serializers/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/serializers/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/assessment/views.py
--rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.006188 ora2-5.0.4/openassessment/fileupload/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.006188 ora2-5.0.4/openassessment/fileupload/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/backends/swift.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/views_django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/fileupload/views_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.006188 ora2-5.0.4/openassessment/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.010188 ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/ar_SA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.010188 ora2-5.0.4/openassessment/locale/ar_SA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.010188 ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.010188 ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.014188 ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94672 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23724 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.014188 ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)   145495 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   195906 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    21982 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38500 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.014188 ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.014188 ora2-5.0.4/openassessment/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.018188 ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.018188 ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.018188 ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.022188 ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.022188 ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.022188 ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.026188 ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.026188 ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.030188 ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.030188 ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.030188 ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.034189 ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.034189 ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/messages.mo
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.034189 ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.038189 ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.038189 ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.042189 ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.042189 ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.990188 ora2-5.0.4/openassessment/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.042189 ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.046189 ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.046189 ora2-5.0.4/openassessment/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.046189 ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/sw_KE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.050189 ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.050189 ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.050189 ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.054189 ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.054189 ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.054189 ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.058189 ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.058189 ora2-5.0.4/openassessment/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.058189 ora2-5.0.4/openassessment/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/commands/collect_ora2_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/commands/create_oa_submissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/commands/create_oa_submissions_from_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/management/commands/upload_oa_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.058189 ora2-5.0.4/openassessment/runtime_imports/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/runtime_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/runtime_imports/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/runtime_imports/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.062189 ora2-5.0.4/openassessment/staffgrader/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.062189 ora2-5.0.4/openassessment/staffgrader/errors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/errors/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.062189 ora2-5.0.4/openassessment/staffgrader/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.062189 ora2-5.0.4/openassessment/staffgrader/models/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/models/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.062189 ora2-5.0.4/openassessment/staffgrader/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/serializers/assessments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/serializers/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/serializers/submission_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/staffgrader/staff_grader_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.066189 ora2-5.0.4/openassessment/templates/openassessmentblock/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.074189 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
--rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
--rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_training_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.074189 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/
--rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.078189 ora2-5.0.4/openassessment/templates/openassessmentblock/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/icons/warning_filled.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.078189 ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.078189 ora2-5.0.4/openassessment/templates/openassessmentblock/leaderboard/
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.082189 ora2-5.0.4/openassessment/templates/openassessmentblock/message/
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_open.html
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_base.html
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_latex_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_submission_answer.html
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/oa_uploaded_file.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/
--rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/response/
--rw-r--r--   0 runner    (1001) docker     (122)    21833 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response.html
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_graded.html
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/self/
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/staff/
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
--rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/
--rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.086189 ora2-5.0.4/openassessment/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/templatetags/oa_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.090189 ora2-5.0.4/openassessment/workflow/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.090189 ora2-5.0.4/openassessment/workflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/migrations/0002_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/migrations/0003_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/workflow/team_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.094189 ora2-5.0.4/openassessment/xblock/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/config_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      914 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/course_items_listing_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/editor_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/grade_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/leaderboard_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/lms_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/load_static.py
--rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/message_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/mobile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/openassesment_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    50871 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/openassessmentblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/peer_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/resolve_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/rubric_reuse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/self_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/staff_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/staff_assessment_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/xblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/xblock/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/xblock/static/css/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.094189 ora2-5.0.4/openassessment/xblock/static/css/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/css/lib/backgrid/backgrid.css
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.130190 ora2-5.0.4/openassessment/xblock/static/dist/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
--rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
--rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.css
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
--rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-07-05 14:20:14.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
--rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.js
--rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
--rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.js
--rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
--rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.js
--rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
--rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/dist/openassessment-studio.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/xblock/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:29.994188 ora2-5.0.4/openassessment/xblock/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.134190 ora2-5.0.4/openassessment/xblock/static/js/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/lib/backgrid/backgrid.js
--rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.134190 ora2-5.0.4/openassessment/xblock/static/js/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.134190 ora2-5.0.4/openassessment/xblock/static/js/src/lms/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.134190 ora2-5.0.4/openassessment/xblock/static/js/src/lms/api/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.134190 ora2-5.0.4/openassessment/xblock/static/js/src/lms/editors/
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_datefactory.js
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_file_upload.js
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_grade.js
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_message.js
--rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_peer.js
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    32835 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_response.js
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_response_editor.js
--rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_self.js
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_staff.js
--rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_staff_area.js
--rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_training.js
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/lms_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    26166 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/oa_server.js
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/oa_shared.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.138190 ora2-5.0.4/openassessment/xblock/static/js/src/studio/
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_container.js
--rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_container_item.js
--rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
--rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
--rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
--rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/static/js/src/studio_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/student_training_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/studio_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    42012 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/submission_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/team_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/team_workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/user_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-07-05 14:20:15.000000 ora2-5.0.4/openassessment/xblock/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.138190 ora2-5.0.4/ora2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23039 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-05 14:20:29.000000 ora2-5.0.4/ora2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:30.138190 ora2-5.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/test-acceptance.in
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-05 14:20:15.000000 ora2-5.0.4/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-05 14:20:30.138190 ora2-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-07-05 14:20:15.000000 ora2-5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.623652 ora2-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-07-05 14:20:58.000000 ora2-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-05 14:20:58.000000 ora2-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-05 14:21:01.623652 ora2-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-05 14:20:58.000000 ora2-5.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/api/teams.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/errors/student_training.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0002_staffworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0003_expand_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0006_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/models/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/score_type_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.547653 ora2-5.1.0/openassessment/assessment/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/serializers/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/serializers/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/assessment/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/fileupload/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/fileupload/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/backends/swift.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/views_django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/fileupload/views_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/ar_SA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/ar_SA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    84892 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27184 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.551653 ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)   145884 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   186603 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    22487 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    42004 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.555653 ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.539653 ora2-5.1.0/openassessment/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/messages.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.559653 ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/sw_KE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.563653 ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/commands/collect_ora2_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/commands/create_oa_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/commands/create_oa_submissions_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/management/commands/upload_oa_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/runtime_imports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/runtime_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/runtime_imports/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/runtime_imports/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.567653 ora2-5.1.0/openassessment/staffgrader/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/staffgrader/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/errors/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/staffgrader/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/staffgrader/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/models/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/staffgrader/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/serializers/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/serializers/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/serializers/submission_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/staffgrader/staff_grader_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/templates/openassessmentblock/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.571653 ora2-5.1.0/openassessment/templates/openassessmentblock/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/icons/warning_filled.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/leaderboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/message/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_open.html
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_latex_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_submission_answer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/
+-rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/response/
+-rw-r--r--   0 runner    (1001) docker     (122)    21492 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/self/
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/staff/
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/
+-rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/
+-rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.575653 ora2-5.1.0/openassessment/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/templatetags/oa_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.579653 ora2-5.1.0/openassessment/workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.579653 ora2-5.1.0/openassessment/workflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/migrations/0002_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/migrations/0003_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/workflow/team_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.579653 ora2-5.1.0/openassessment/xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/config_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/course_items_listing_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/editor_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/grade_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/leaderboard_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/lms_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/load_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/message_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/openassesment_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50871 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/openassessmentblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/peer_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/resolve_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/rubric_reuse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/self_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/staff_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/staff_assessment_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/xblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/xblock/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/xblock/static/css/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.579653 ora2-5.1.0/openassessment/xblock/static/css/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.615652 ora2-5.1.0/openassessment/xblock/static/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
+-rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1350843 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.css
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
+-rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757664 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (122)   757693 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235851 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/dist/openassessment-studio.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/xblock/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.543653 ora2-5.1.0/openassessment/xblock/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.619652 ora2-5.1.0/openassessment/xblock/static/js/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.619652 ora2-5.1.0/openassessment/xblock/static/js/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.619652 ora2-5.1.0/openassessment/xblock/static/js/src/lms/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.619652 ora2-5.1.0/openassessment/xblock/static/js/src/lms/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.619652 ora2-5.1.0/openassessment/xblock/static/js/src/lms/editors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_grade.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_message.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_peer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32903 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_response.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_self.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_staff.js
+-rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_training.js
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/lms_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26171 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/oa_server.js
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/oa_shared.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.623652 ora2-5.1.0/openassessment/xblock/static/js/src/studio/
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_container_item.js
+-rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/static/js/src/studio_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/student_training_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/studio_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41983 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/submission_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/team_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/team_workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-07-05 14:20:58.000000 ora2-5.1.0/openassessment/xblock/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.623652 ora2-5.1.0/ora2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23584 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-05 14:21:01.000000 ora2-5.1.0/ora2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:21:01.623652 ora2-5.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/test-acceptance.in
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-05 14:20:58.000000 ora2-5.1.0/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-05 14:21:01.623652 ora2-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-07-05 14:20:58.000000 ora2-5.1.0/setup.py
```

### Comparing `ora2-5.0.4/LICENSE` & `ora2-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/MANIFEST.in` & `ora2-5.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/PKG-INFO` & `ora2-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.4
+Version: 5.1.0
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.4/README.rst` & `ora2-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/admin.py` & `ora2-5.1.0/openassessment/assessment/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/api/peer.py` & `ora2-5.1.0/openassessment/assessment/api/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/api/self.py` & `ora2-5.1.0/openassessment/assessment/api/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/api/staff.py` & `ora2-5.1.0/openassessment/assessment/api/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/api/student_training.py` & `ora2-5.1.0/openassessment/assessment/api/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/api/teams.py` & `ora2-5.1.0/openassessment/assessment/api/teams.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/errors/peer.py` & `ora2-5.1.0/openassessment/assessment/errors/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/errors/self.py` & `ora2-5.1.0/openassessment/assessment/errors/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/errors/staff.py` & `ora2-5.1.0/openassessment/assessment/errors/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0001_initial.py` & `ora2-5.1.0/openassessment/assessment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0002_staffworkflow.py` & `ora2-5.1.0/openassessment/assessment/migrations/0002_staffworkflow.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0003_expand_course_id.py` & `ora2-5.1.0/openassessment/assessment/migrations/0003_expand_course_id.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py` & `ora2-5.1.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py` & `ora2-5.1.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0006_TeamWorkflows.py` & `ora2-5.1.0/openassessment/assessment/migrations/0006_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/migrations/0007_staff_workflow_blank.py` & `ora2-5.1.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/models/base.py` & `ora2-5.1.0/openassessment/assessment/models/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/models/peer.py` & `ora2-5.1.0/openassessment/assessment/models/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/models/staff.py` & `ora2-5.1.0/openassessment/assessment/models/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/models/student_training.py` & `ora2-5.1.0/openassessment/assessment/models/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/models/training.py` & `ora2-5.1.0/openassessment/assessment/models/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/serializers/base.py` & `ora2-5.1.0/openassessment/assessment/serializers/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/serializers/peer.py` & `ora2-5.1.0/openassessment/assessment/serializers/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/serializers/training.py` & `ora2-5.1.0/openassessment/assessment/serializers/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/assessment/views.py` & `ora2-5.1.0/openassessment/assessment/views.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/data.py` & `ora2-5.1.0/openassessment/data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/api.py` & `ora2-5.1.0/openassessment/fileupload/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/__init__.py` & `ora2-5.1.0/openassessment/fileupload/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/base.py` & `ora2-5.1.0/openassessment/fileupload/backends/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/django_storage.py` & `ora2-5.1.0/openassessment/fileupload/backends/django_storage.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/filesystem.py` & `ora2-5.1.0/openassessment/fileupload/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/s3.py` & `ora2-5.1.0/openassessment/fileupload/backends/s3.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/backends/swift.py` & `ora2-5.1.0/openassessment/fileupload/backends/swift.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/exceptions.py` & `ora2-5.1.0/openassessment/fileupload/exceptions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/fileupload/views_filesystem.py` & `ora2-5.1.0/openassessment/fileupload/views_filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/el/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
-# EdX Team <info@edx.org>, 2018.
-#
+# 
+# Translators:
+# Buyandelger Batbayar <buyka.1776@gmail.com>, 2021
+# Jamka Sukhee <jambka.93@gmail.com>, 2021
+# Mendbayar Gantulga <mendbayar_mgo@yahoo.com>, 2021
+# Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021
 msgid ""
 msgstr ""
-"Project-Id-Version: edx-ora2\n"
+"Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-09-13 04:00-0400\n"
-"PO-Revision-Date: 2014-06-04 15:41-0400\n"
-"Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: openedx-translation <openedx-translation@googlegroups.com>\n"
-"Language: en\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
+"PO-Revision-Date: 2014-06-11 13:03+0000\n"
+"Last-Translator: Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021\n"
+"Language-Team: Mongolian (http://app.transifex.com/open-edx/edx-platform/language/mn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: mn\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
-"If your assignment includes a learner training step, the rubric must have at "
-"least one criterion, and that criterion must have at least one option."
+"If your assignment includes a learner training step, the rubric must have at"
+" least one criterion, and that criterion must have at least one option."
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:203
 #, python-brace-format
 msgid "Example {example_number} has a validation error: {error}"
 msgstr ""
 
@@ -148,17 +153,18 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
-"Open Response Assessments allow you to configure single or multiple steps in "
-"a rubric based open response assessment sequence. The steps available below "
-"can be enabled, disable, and ordered for a flexible set of pedagogical needs."
+"Open Response Assessments allow you to configure single or multiple steps in"
+" a rubric based open response assessment sequence. The steps available below"
+" can be enabled, disable, and ordered for a flexible set of pedagogical "
+"needs."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:5
 msgid "Display Name "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:8
@@ -245,16 +251,16 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:70
 msgid "File Types"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:79
 msgid ""
-"Enter the file extensions, separated by commas, that you want learners to be "
-"able to upload. For example: pdf,doc,docx."
+"Enter the file extensions, separated by commas, that you want learners to be"
+" able to upload. For example: pdf,doc,docx."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:84
 msgid ""
 "To add more file extensions, select Custom File Types and enter the full "
 "list of acceptable file extensions to be included."
 msgstr ""
@@ -275,17 +281,17 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:104
 msgid " (Disabled)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:117
 msgid ""
-"Specify the number of top scoring responses to display after the learner has "
-"submitted a response. Valid numbers are 0 to 99. If the number is 0, the Top "
-"Responses section does not appear to learners."
+"Specify the number of top scoring responses to display after the learner has"
+" submitted a response. Valid numbers are 0 to 99. If the number is 0, the "
+"Top Responses section does not appear to learners."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:122
 msgid "When Teams Enabled is set to true, Top Responses will be disabled."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:129
@@ -364,15 +370,15 @@
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:3
 msgid "Open Response Assessment"
-msgstr ""
+msgstr "Нээлттэй хариулах асуултын үнэлгээ"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:8
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:7
 msgid "Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:15
@@ -385,15 +391,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr ""
+msgstr "Тохиргоо"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
@@ -416,16 +422,16 @@
 "Peer Assessment allows students to provide feedback to other students and "
 "also receive feedback from others in their final grade. Often, though not "
 "always, this step is preceded by Self Assessment or Learner Training steps."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:18
 msgid ""
-"Configuration: For this step to be configured you must specify the number of "
-"peer reviews a student will be assessed with, and the number of peer a "
+"Configuration: For this step to be configured you must specify the number of"
+" peer reviews a student will be assessed with, and the number of peer a "
 "student must grade. Additional options can be specified."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:23
 msgid "View Options & Configuration"
 msgstr ""
 
@@ -441,16 +447,16 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:36
 msgid "Graded By"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:39
 msgid ""
-"Specify the number of learners that each response must be assessed by. Valid "
-"numbers are 1 to 99."
+"Specify the number of learners that each response must be assessed by. Valid"
+" numbers are 1 to 99."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:43
 msgid "Enable Flexible Peer Grade Averaging"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:49
@@ -524,16 +530,16 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:40
 msgid "Feedback Instructions"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:44
 msgid ""
-"Encourage learners to provide feedback on the response they have graded. You "
-"can replace the sample text with your own."
+"Encourage learners to provide feedback on the response they have graded. You"
+" can replace the sample text with your own."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:49
 msgid "Default Feedback Text"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:53
@@ -612,16 +618,16 @@
 "submission in order to train them on the rubric and ensure learner's "
 "understand the rubric for either Self or Peer Assessment steps."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:17
 msgid ""
 "Configuration: For this step to be fully configured you must provide one or "
-"more graded sample responses. Learners must then match this instructor score "
-"to advance and are provided feedback when their score doesn't match the "
+"more graded sample responses. Learners must then match this instructor score"
+" to advance and are provided feedback when their score doesn't match the "
 "sample response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:22
 msgid "View / Add Sample Responses"
 msgstr ""
 
@@ -667,15 +673,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr ""
+msgstr "Хариулт"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
@@ -683,16 +689,15 @@
 msgid "points"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
-"                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - "
-"%(grade)s%(end_tag)s\n"
+"                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:7
 #, python-format
 msgid ""
 "\n"
@@ -713,50 +718,48 @@
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
 msgid "Your Grade"
-msgstr ""
+msgstr "Таны Оноо"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:19
 #, python-format
 msgid ""
 "\n"
-"                                        %(points_earned)s out of "
-"%(points_possible)s\n"
+"                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:38
 msgid "Your submission has been cancelled."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:19
 #, python-format
 msgid ""
 "\n"
-"                                            %(points_earned)s out of "
-"%(points_possible)s\n"
+"                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr ""
+msgstr "Таны хариулт"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
-msgstr ""
+msgstr "Таны хариултын үнэлгээ"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:50
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:132
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:28
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:28
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:4
 #: openassessment/templates/openassessmentblock/message/oa_message_closed.html:4
@@ -846,15 +849,15 @@
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr ""
+msgstr "Дуусаагүй"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
@@ -918,16 +921,16 @@
 msgid ""
 "After you complete all the steps of this assignment, you can see the top-"
 "scoring responses from your peers."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:8
 msgid ""
-"Your team’s submission has been cancelled. Your team will receive a grade of "
-"zero unless course staff resets your assessment to allow the team to "
+"Your team’s submission has been cancelled. Your team will receive a grade of"
+" zero unless course staff resets your assessment to allow the team to "
 "resubmit a response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:10
 msgid ""
 "Your submission has been cancelled. You will receive a grade of zero unless "
 "course staff resets your assessment to allow you to resubmit a response."
@@ -976,119 +979,101 @@
 "has started."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:20
 #, python-format
 msgid ""
 "\n"
-"                                    %(start_strong)sThis assignment is in "
-"progress. The self assessment step will close soon.%(end_strong)s You still "
-"need to complete the %(start_link)sself assessment%(end_link)s step.\n"
+"                                    %(start_strong)sThis assignment is in progress. The self assessment step will close soon.%(end_strong)s You still need to complete the %(start_link)sself assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:24
 #, python-format
 msgid ""
 "\n"
-"                                    This assignment is in progress. You "
-"still need to complete the %(start_link)sself assessment%(end_link)s step.\n"
+"                                    This assignment is in progress. You still need to complete the %(start_link)sself assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:38
 #, python-format
 msgid ""
 "\n"
-"                                    This assignment is in progress."
-"%(start_strong)sThe peer assessment step will close soon.%(end_strong)s All "
-"submitted peer responses have been assessed. Check back later to see if more "
-"learners have submitted responses. You still need to complete the "
-"%(start_link)speer assessment%(end_link)s step.\n"
+"                                    This assignment is in progress.%(start_strong)sThe peer assessment step will close soon.%(end_strong)s All submitted peer responses have been assessed. Check back later to see if more learners have submitted responses. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:42
 #, python-format
 msgid ""
 "\n"
-"                                    This assignment is in progress. All "
-"submitted peer responses have been assessed. Check back later to see if more "
-"learners have submitted responses. You still need to complete the "
-"%(start_link)speer assessment%(end_link)s step.\n"
+"                                    This assignment is in progress. All submitted peer responses have been assessed. Check back later to see if more learners have submitted responses. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:46
 #, python-format
 msgid ""
 "\n"
-"                                    This assignment is in progress. "
-"%(start_strong)sThe peer assessment step will close soon.%(end_strong)s You "
-"still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
+"                                    This assignment is in progress. %(start_strong)sThe peer assessment step will close soon.%(end_strong)s You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html:50
 #, python-format
 msgid ""
 "\n"
-"                                    This assignment is in progress. You "
-"still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
+"                                    This assignment is in progress. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_no_team.html:4
 msgid "Team membership is required to view this assignment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_no_team.html:7
 #, python-format
 msgid ""
 "\n"
 "            This is a team assignment for team-set \"%(teamset_name)s\".\n"
-"            You are currently not on a team in team-set "
-"\"%(teamset_name)s\".\n"
-"            You must be on a team in team-set \"%(teamset_name)s\" to access "
-"this team assignment.\n"
+"            You are currently not on a team in team-set \"%(teamset_name)s\".\n"
+"            You must be on a team in team-set \"%(teamset_name)s\" to access this team assignment.\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_open.html:7
 #, python-format
 msgid ""
 "\n"
-"                    Assignment submissions will close soon. To receive a "
-"grade, first provide a response to the prompt, then complete the steps below "
-"the %(start_tag)sYour Response%(end_tag)s field.\n"
+"                    Assignment submissions will close soon. To receive a grade, first provide a response to the prompt, then complete the steps below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_open.html:11
 #, python-format
 msgid ""
 "\n"
-"                    This assignment has several steps. In the first step, "
-"you'll provide a response to the prompt. The other steps appear below the "
-"%(start_tag)sYour Response%(end_tag)s field.\n"
+"                    This assignment has several steps. In the first step, you'll provide a response to the prompt. The other steps appear below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:4
 msgid "Instructions Unavailable"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:6
 msgid "The instructions for this step could not be loaded."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:15
 msgid ""
 "This assignment has several steps. In the first step, you'll provide a "
-"response to the prompt. The other steps appear below the Your Response field."
+"response to the prompt. The other steps appear below the Your Response "
+"field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
@@ -1105,15 +1090,15 @@
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
-msgstr ""
+msgstr "Энэ хэсгийн асуулт"
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:27
 #: openassessment/templates/openassessmentblock/oa_uploaded_file.html:34
@@ -1135,35 +1120,33 @@
 "administrator. If you access the files, you do so at your own risk.)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:26
 msgid "Assess Peers"
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "available August 13th, 2014 00:00 UTC (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "available August 13th, 2014 00:00 UTC (in
+#. 5 days and 45 minutes)"
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:34
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" "
-"data-datetime=\"%(start_date)s\" data-string=\"available {date} (in "
-"%(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "due August 13th, 2014 00:00 UTC (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "due August 13th, 2014 00:00 UTC (in 5 days
+#. and 45 minutes)"
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:41
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" "
-"data-datetime=\"%(due_date)s\" data-string=\"due {date} (in "
-"%(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:51
 #, python-format
 msgid ""
 "\n"
@@ -1214,15 +1197,15 @@
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr ""
+msgstr "Гүйцээсэн"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
@@ -1269,43 +1252,41 @@
 "        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html:37
 msgid ""
 "All available peer responses have been assessed. Check back later to see if "
 "more learners have submitted responses. You will receive your grade after "
-"you've completed all the steps for this problem and your peers have assessed "
-"your response."
+"you've completed all the steps for this problem and your peers have assessed"
+" your response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:27
 msgid "Your Team's Response"
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "available August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "available August 13th, 2014 (in 5 days and
+#. 45 minutes)"
 #: openassessment/templates/openassessmentblock/response/oa_response.html:39
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline_response\" class=\"date ora-"
-"datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} "
-"(in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "due August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
+#. minutes)"
 #: openassessment/templates/openassessmentblock/response/oa_response.html:46
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline_response\" class=\"date ora-"
-"datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in "
-"%(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
 msgstr ""
@@ -1313,40 +1294,38 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
 "\n"
-"                        You can save your progress and return to complete "
-"your team's response at any time before the due date\n"
+"                        You can save your progress and return to complete your team's response at any time before the due date\n"
 "                      "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:81
 msgid ""
 "\n"
-"                        You can save your progress and return to complete "
-"your team's response at any time.\n"
+"                        You can save your progress and return to complete your team's response at any time.\n"
 "                      "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:86
-msgid "After you submit a response on behalf of your team, it cannot be edited"
+msgid ""
+"After you submit a response on behalf of your team, it cannot be edited"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:89
 msgid "Enter your response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:91
 msgid ""
 "\n"
-"                        You can save your progress and return to complete "
-"your response at any time before the due date\n"
+"                        You can save your progress and return to complete your response at any time before the due date\n"
 "                      "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:104
 msgid ""
 "You can save your progress and return to complete your response at any time."
 msgstr ""
@@ -1372,18 +1351,16 @@
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:151
 #, python-format
 msgid ""
 "\n"
 "                                              %(team_members_with_external_submissions)s\n"
-"                                              have/has already submitted a "
-"response to this assignment with another team,\n"
-"                                              and will not be a part of your "
-"team's submission or assignment grade.\n"
+"                                              have/has already submitted a response to this assignment with another team,\n"
+"                                              and will not be a part of your team's submission or assignment grade.\n"
 "                                          "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:167
 msgid "Team Response "
 msgstr ""
 
@@ -1400,42 +1377,34 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:246
 msgid "(Optional)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:179
 msgid ""
 "\n"
-"                                              Teams should designate one "
-"team member to submit a response on behalf of the\n"
-"                                              entire team.  All team members "
-"can use this space to work on draft responses,\n"
-"                                              but you will not be able to "
-"see your teammates' drafts made in this space, so\n"
-"                                              please coordinate with them to "
-"decide on the final response the designated team\n"
+"                                              Teams should designate one team member to submit a response on behalf of the\n"
+"                                              entire team.  All team members can use this space to work on draft responses,\n"
+"                                              but you will not be able to see your teammates' drafts made in this space, so\n"
+"                                              please coordinate with them to decide on the final response the designated team\n"
 "                                              member should submit.\n"
 "                                          "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:194
 msgid "Enter your response to the prompt above."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:208
 #, python-format
 msgid ""
 "\n"
-"                                      You are currently on Team "
-"%(team_name)s. Since you were on Team %(previous_team_name)s\n"
-"                                      when they submitted a response to this "
-"assignment, you are seeing Team %(previous_team_name)s’s\n"
-"                                      response and will receive the same "
-"grade for this assignment as your former teammates.\n"
-"                                      You will not be part of Team "
-"%(team_name)s’s submission for this assignment and will not\n"
+"                                      You are currently on Team %(team_name)s. Since you were on Team %(previous_team_name)s\n"
+"                                      when they submitted a response to this assignment, you are seeing Team %(previous_team_name)s’s\n"
+"                                      response and will receive the same grade for this assignment as your former teammates.\n"
+"                                      You will not be part of Team %(team_name)s’s submission for this assignment and will not\n"
 "                                      receive a grade for their submission.\n"
 "                                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:221
 msgid "We could not save your progress"
 msgstr ""
@@ -1451,18 +1420,16 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:242
 msgid "File Uploads "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:250
 msgid ""
 "\n"
-"                                  Upload files and review files uploaded by "
-"you and your teammates below. Be sure to add\n"
-"                                  descriptions to your files to help your "
-"teammates identify them.\n"
+"                                  Upload files and review files uploaded by you and your teammates below. Be sure to add\n"
+"                                  descriptions to your files to help your teammates identify them.\n"
 "                              "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:258
 msgid "We could not upload files"
 msgstr ""
 
@@ -1518,18 +1485,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:314
 msgid "One team member should submit on behalf of the entire team."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:316
 msgid ""
 "\n"
-"                  Learn more about team assignments here: (<a "
-"target=\"_blank\" href=\"https://support.edx.org/hc/en-us/"
-"articles/360000191067-Submit-your-"
-"response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
+"                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
 msgstr ""
 
@@ -1541,25 +1505,23 @@
 msgid "Your submission was cancelled. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:37
 #, python-format
 msgid ""
 "\n"
-"                                Your submission has been cancelled by "
-"%(removed_by_username)s on %(removed_datetime)s\n"
+"                                Your submission has been cancelled by %(removed_by_username)s on %(removed_datetime)s\n"
 "                            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:41
 #, python-format
 msgid ""
 "\n"
-"                               Your submission was cancelled on "
-"%(removed_datetime)s\n"
+"                               Your submission was cancelled on %(removed_datetime)s\n"
 "                            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:48
 #, python-format
 msgid ""
 "\n"
@@ -1572,16 +1534,16 @@
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
-"longer submit a response or continue with this problem, and you will receive "
-"a grade of Incomplete. If you saved but did not submit a response, the "
+"longer submit a response or continue with this problem, and you will receive"
+" a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:20
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:20
 #: openassessment/templates/openassessmentblock/self/oa_self_complete.html:18
 #: openassessment/templates/openassessmentblock/student_training/student_training_complete.html:17
@@ -1607,81 +1569,72 @@
 "steps are complete and your response is fully assessed."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:34
 #, python-format
 msgid ""
 "\n"
-"                        You still need to complete the "
-"%(peer_start_tag)speer assessment%(end_tag)s and %(self_start_tag)sself "
-"assessment%(end_tag)s steps.\n"
+"                        You still need to complete the %(peer_start_tag)speer assessment%(end_tag)s and %(self_start_tag)sself assessment%(end_tag)s steps.\n"
 "                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:38
 #, python-format
 msgid ""
 "\n"
-"                        You still need to complete the %(start_tag)speer "
-"assessment%(end_tag)s step.\n"
+"                        You still need to complete the %(start_tag)speer assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:42
 #, python-format
 msgid ""
 "\n"
-"                        You still need to complete the %(start_tag)sself "
-"assessment%(end_tag)s step.\n"
+"                        You still need to complete the %(start_tag)sself assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:15
 msgid "Error"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:29
 #, python-format
 msgid ""
 "\n"
-"                            You joined Team %(team_name)s after they "
-"submitted a response for this assignment\n"
-"                            and you will not receive a grade for their "
-"response. You have also not previously submitted\n"
-"                            a response to this assignment with another team. "
-"Please contact course staff to discuss your\n"
+"                            You joined Team %(team_name)s after they submitted a response for this assignment\n"
+"                            and you will not receive a grade for their response. You have also not previously submitted\n"
+"                            a response to this assignment with another team. Please contact course staff to discuss your\n"
 "                            options for this assignment.\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:23
 msgid "Assess Your Response"
-msgstr ""
+msgstr "Таны хариултын үнэлгээ"
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "available August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "available August 13th, 2014 (in 5 days and
+#. 45 minutes)"
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:31
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"               <span id=\"oa_step_deadline_self\" class=\"date ora-"
-"datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} "
-"(in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "           "
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "due August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
+#. minutes)"
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:38
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"               <span id=\"oa_step_deadline_self\" class=\"date ora-"
-"datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in "
-"%(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "           "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:78
 msgid "Submit your assessment"
 msgstr ""
 
@@ -1787,16 +1740,15 @@
 msgid "Give this learner a grade using the problem's rubric."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:26
 #, python-format
 msgid ""
 "\n"
-"                                        Response for: %(team_name)s with "
-"%(team_usernames)s\n"
+"                                        Response for: %(team_name)s with %(team_usernames)s\n"
 "                                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:30
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:20
 #, python-format
 msgid ""
@@ -1878,25 +1830,23 @@
 msgid "Team's Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:39
 #, python-format
 msgid ""
 "\n"
-"                            Learner submission removed by "
-"%(removed_by_username)s on %(removed_datetime)s\n"
+"                            Learner submission removed by %(removed_by_username)s on %(removed_datetime)s\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:43
 #, python-format
 msgid ""
 "\n"
-"                            Learner submission removed on "
-"%(removed_datetime)s\n"
+"                            Learner submission removed on %(removed_datetime)s\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:50
 #, python-format
 msgid ""
 "\n"
@@ -1932,34 +1882,31 @@
 msgid "Team's Final Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:112
 #, python-format
 msgid ""
 "\n"
-"                            Final grade: %(points_earned)s out of "
-"%(points_possible)s\n"
+"                            Final grade: %(points_earned)s out of %(points_possible)s\n"
 "                        "
-msgstr ""
+msgstr "\nЭцсийн үнэлгээ: %(points_possible)s онооноос %(points_earned)s"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:119
 msgid "Final Grade Details"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:139
 #, python-format
 msgid ""
 "\n"
-"                                        %(assessment_label)s - %(points)s "
-"point\n"
+"                                        %(assessment_label)s - %(points)s point\n"
 "                                    "
 msgid_plural ""
 "\n"
-"                                        %(assessment_label)s - %(points)s "
-"points\n"
+"                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
 msgstr[0] ""
 msgstr[1] ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
@@ -1974,16 +1921,16 @@
 "receives a grade of zero unless you delete the learner's state for the "
 "problem to allow them to resubmit a response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:172
 msgid ""
 "The team’s submission has been removed from grading. The team receives a "
-"grade of zero unless you delete the a team member’s state for the problem to "
-"allow the team to resubmit a response."
+"grade of zero unless you delete the a team member’s state for the problem to"
+" allow the team to resubmit a response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:177
 msgid "The problem has not been started."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:181
@@ -2065,54 +2012,51 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:26
 msgid "Selected Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
-msgstr ""
+msgstr "Санал шүүмж"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:27
 #, python-format
 msgid ""
 "\n"
-"                      In Progress (%(current_progress_num)s of "
-"%(training_available_num)s)\n"
+"                      In Progress (%(current_progress_num)s of %(training_available_num)s)\n"
 "                  "
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "available August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "available August 13th, 2014 (in 5 days and
+#. 45 minutes)"
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:38
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-"
-"datetime=\"%(start_date)s\" data-string=\"available {date} (in "
-"%(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-"
-"language=\"%(user_language)s\"></span>\n"
+"            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
-#. Translators: This string displays a date to the user, then tells them the time until that date.  Example: "due August 13th, 2014 (in 5 days and 45 minutes)"
+#. Translators: This string displays a date to the user, then tells them the
+#. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
+#. minutes)"
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:45
 #, python-format, python-brace-format
 msgid ""
 "\n"
-"            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-"
-"datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" "
-"data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></"
-"span>\n"
+"            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:58
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:66
 msgid "Learning to Assess Responses"
 msgstr ""
@@ -2146,15 +2090,16 @@
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:105
 msgid "Selected Options Differ"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:108
-msgid "The option you selected is not the option that the instructor selected."
+msgid ""
+"The option you selected is not the option that the instructor selected."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:144
 msgid "We could not check your assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:151
@@ -2233,15 +2178,15 @@
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Self Assessment Grade"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Your Self Assessment"
-msgstr ""
+msgstr "Таны өөрийгөө үнэлэх үнэлгээ"
 
 #: openassessment/xblock/grade_mixin.py:385
 #: openassessment/xblock/grade_mixin.py:527
 msgid "Your Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:481
@@ -2265,22 +2210,22 @@
 #: openassessment/xblock/grade_mixin.py:656
 msgid "The grade for this problem is determined by your Self Assessment."
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:662
 #, python-brace-format
 msgid ""
-"You have successfully completed this problem and received a {earned_points}/"
-"{total_points}."
-msgstr ""
+"You have successfully completed this problem and received a "
+"{earned_points}/{total_points}."
+msgstr "Та энэ дасгалыг амжилттай дуусгаж {earned_points}/{total_points} оноо авлаа."
 
 #: openassessment/xblock/grade_mixin.py:670
 msgid ""
-"You have not yet received all necessary peer reviews to determine your final "
-"grade."
+"You have not yet received all necessary peer reviews to determine your final"
+" grade."
 msgstr ""
 
 #: openassessment/xblock/openassesment_template_mixin.py:19
 msgid "Peer Assessment Only"
 msgstr ""
 
 #: openassessment/xblock/openassesment_template_mixin.py:20
@@ -2493,16 +2438,16 @@
 
 #: openassessment/xblock/staff_assessment_mixin.py:190
 msgid "Waiting for a Staff Grade"
 msgstr ""
 
 #: openassessment/xblock/staff_assessment_mixin.py:191
 msgid ""
-"Check back later to see if a course staff member has assessed your response. "
-"You will receive your grade after the assessment is complete."
+"Check back later to see if a course staff member has assessed your response."
+" You will receive your grade after the assessment is complete."
 msgstr ""
 
 #: openassessment/xblock/staff_assessment_mixin.py:204
 msgid "You Must Complete the Steps Above to View Your Grade"
 msgstr ""
 
 #: openassessment/xblock/staff_assessment_mixin.py:205
@@ -2630,16 +2575,15 @@
 msgstr ""
 
 #: openassessment/xblock/validation.py:122
 msgid "The assessment order you selected is invalid."
 msgstr ""
 
 #: openassessment/xblock/validation.py:132
-msgid ""
-"In peer assessment, the \"Must Grade\" value must be a positive integer."
+msgid "In peer assessment, the \"Must Grade\" value must be a positive integer."
 msgstr ""
 
 #: openassessment/xblock/validation.py:135
 msgid "In peer assessment, the \"Graded By\" value must be a positive integer."
 msgstr ""
 
 #: openassessment/xblock/validation.py:139
@@ -2653,16 +2597,15 @@
 msgstr ""
 
 #: openassessment/xblock/validation.py:151
 msgid "Each example response for learner training must be unique."
 msgstr ""
 
 #: openassessment/xblock/validation.py:158
-msgid ""
-"The \"required\" value must be true if staff assessment is the only step."
+msgid "The \"required\" value must be true if staff assessment is the only step."
 msgstr ""
 
 #: openassessment/xblock/validation.py:162
 msgid ""
 "The number of assessments cannot be changed after the problem has been "
 "released."
 msgstr ""
```

### Comparing `ora2-5.0.4/openassessment/locale/en/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
-# EdX Team <info@edx.org>, 2018.
-#
+# 
+# Translators:
 msgid ""
 msgstr ""
-"Project-Id-Version: edx-ora2\n"
+"Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
-"PO-Revision-Date: 2014-06-04 15:41-0400\n"
+"PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: openedx-translation <openedx-translation@googlegroups.com>\n"
-"Language: en\n"
+"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/language/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: lv\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : 2);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
@@ -151,15 +151,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr ""
+msgstr "Aktivitātes"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -197,15 +197,15 @@
 msgid "Waiting"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr ""
+msgstr "Personāls"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
 msgstr ""
 
@@ -219,15 +219,15 @@
 msgid "List of Open Assessments is unavailable"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr ""
+msgstr "Lūdzu, uzgaidiet"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -276,15 +276,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr ""
+msgstr "Kļūda"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -298,16 +298,16 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:590
 msgid ""
-"File upload failed: unsupported file type. Only the supported file types can "
-"be uploaded. If you have questions, please reach out to the course team."
+"File upload failed: unsupported file type. Only the supported file types can"
+" be uploaded. If you have questions, please reach out to the course team."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
 msgstr ""
 
@@ -431,66 +431,66 @@
 msgid ""
 "There are currently {stuck_learners} learners in the waiting state, meaning "
 "they have not yet met all requirements for Peer Assessment. "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
-"However, {overwritten_count} of these students have received a grade through "
-"the staff grade override tool already."
+"However, {overwritten_count} of these students have received a grade through"
+" the staff grade override tool already."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr ""
+msgstr "Paragrāfs"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr ""
+msgstr "Iepriekš formatēts"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr ""
+msgstr "Virsraksts 3"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr ""
+msgstr "Virsraksts 4"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr ""
+msgstr "Virsraksts 5"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr ""
+msgstr "Virsraksts 6"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr ""
+msgstr "Nav izvēlēts"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
@@ -543,16 +543,16 @@
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
-"Changes to steps that are not selected as part of the assignment will not be "
-"saved."
+"Changes to steps that are not selected as part of the assignment will not be"
+" saved."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
 msgstr ""
 
@@ -569,15 +569,15 @@
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 msgid ""
-"This ORA has already been released. Changes will only affect learners making "
-"new submissions. Existing submissions will not be modified by this change."
+"This ORA has already been released. Changes will only affect learners making"
+" new submissions. Existing submissions will not be modified by this change."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:318
 msgid "error count: "
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -369,59 +369,14 @@
 msgstr ""
 "\n"
 "                        Çömménts: %(comments)s\n"
 "                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
 msgid ""
 "\n"
-"                        You can save your progress and return to complete "
-"your response at any time before the due date\n"
-"                      "
-msgstr ""
-"\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété "
-"ýöür réspönsé ät äný tïmé ßéföré thé düé däté\n"
-"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
-"єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
-"єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
-"αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
-"νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
-"σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт "
-"αηιм ι∂ єѕ#"
-
-msgid ""
-"\n"
-"                        You can save your progress and return to complete "
-"your team's response at any time before the due date\n"
-"                      "
-msgstr ""
-"\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété "
-"ýöür téäm's réspönsé ät äný tïmé ßéföré thé düé däté\n"
-"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
-"єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
-"єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
-"αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
-"νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
-"σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт "
-"αη#"
-
-msgid ""
-"\n"
-"                        You can save your progress and return to complete "
-"your team's response at any time.\n"
-"                      "
-msgstr ""
-"\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété "
-"ýöür téäm's réspönsé ät äný tïmé.\n"
-"                       Ⱡ#"
-
-msgid ""
-"\n"
 "                        You still need to complete the "
 "%(peer_start_tag)speer assessment%(end_tag)s and %(self_start_tag)sself "
 "assessment%(end_tag)s steps.\n"
 "                    "
 msgstr ""
 "\n"
 "                        Ýöü stïll nééd tö çömplété thé "
@@ -449,14 +404,63 @@
 "\n"
 "                        Ýöü stïll nééd tö çömplété thé %(start_tag)ssélf "
 "ässéssmént%(end_tag)s stép.\n"
 "                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
 msgid ""
 "\n"
+"                        Your work will save automatically and you can return "
+"to complete your response at any time before the due date\n"
+"                      "
+msgstr ""
+"\n"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn "
+"tö çömplété ýöür réspönsé ät äný tïmé ßéföré thé düé däté\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
+"єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
+"єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
+"αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
+"νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
+"σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт#"
+
+msgid ""
+"\n"
+"                        Your work will save automatically and you can return "
+"to complete your team's response at any time before the due date\n"
+"                      "
+msgstr ""
+"\n"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn "
+"tö çömplété ýöür téäm's réspönsé ät äný tïmé ßéföré thé düé däté\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
+"єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
+"єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
+"αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
+"νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
+"σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια#"
+
+msgid ""
+"\n"
+"                        Your work will save automatically and you can return "
+"to complete your team's response at any time.\n"
+"                      "
+msgstr ""
+"\n"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn "
+"tö çömplété ýöür téäm's réspönsé ät äný tïmé.\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
+"єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
+"єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
+"αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
+"νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
+"σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт "
+"αηιм ι#"
+
+msgid ""
+"\n"
 "                      %(assessment_title)s - %(points)s point\n"
 "                  "
 msgid_plural ""
 "\n"
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
 msgstr[0] ""
@@ -805,17 +809,18 @@
 msgid ""
 "After you complete all the steps of this assignment, you can see the top-"
 "scoring responses from your peers."
 msgstr ""
 "Àftér ýöü çömplété äll thé stéps öf thïs ässïgnmént, ýöü çän séé thé töp-"
 "sçörïng réspönsés fröm ýöür péérs. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-msgid "After you submit a response on behalf of your team, it cannot be edited"
+msgid ""
+"After you submit a response on behalf of your team, it cannot be edited."
 msgstr ""
-"Àftér ýöü süßmït ä réspönsé ön ßéhälf öf ýöür téäm, ït çännöt ßé édïtéd "
+"Àftér ýöü süßmït ä réspönsé ön ßéhälf öf ýöür téäm, ït çännöt ßé édïtéd. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
 msgid "After you submit your response, you cannot edit it"
 msgstr ""
 "Àftér ýöü süßmït ýöür réspönsé, ýöü çännöt édït ït Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
@@ -1092,14 +1097,17 @@
 
 msgid "Demo the new Grading Experience"
 msgstr "Démö thé néw Grädïng Éxpérïénçé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
 msgid "Display Name "
 msgstr "Dïspläý Nämé  Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
+msgid "Draft saved!"
+msgstr "Dräft sävéd! Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+
 msgid "Due Date"
 msgstr "Düé Däté Ⱡ'σяєм ιρѕυм ∂#"
 
 msgid "Due Time"
 msgstr "Düé Tïmé Ⱡ'σяєм ιρѕυм ∂#"
 
 msgid "Each example response for learner training must be unique."
@@ -1668,14 +1676,17 @@
 
 msgid "Peer {peer_index}"
 msgstr "Péér {peer_index} Ⱡ'σяєм ιρѕυм ∂#"
 
 msgid "Pending"
 msgstr "Péndïng Ⱡ'σяєм ιρѕυм #"
 
+msgid "Please contact support staff."
+msgstr "Pléäsé çöntäçt süppört stäff. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
+
 msgid "Please enter valid reason to remove the submission."
 msgstr ""
 "Pléäsé éntér välïd réäsön tö rémövé thé süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
 msgid "Please wait"
 msgstr "Pléäsé wäït Ⱡ'σяєм ιρѕυм ∂σłσя #"
@@ -1792,14 +1803,17 @@
 msgstr "Réspönsé Stärt Tïmé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
 msgid "Response exceeds maximum allowed size."
 msgstr ""
 "Réspönsé éxçééds mäxïmüm ällöwéd sïzé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
+msgid "Response not started."
+msgstr "Réspönsé nöt stärtéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
+
 msgid "Response total"
 msgstr "Réspönsé tötäl Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
 msgid "Rubric"
 msgstr "Rüßrïç Ⱡ'σяєм ιρѕυ#"
 
 msgid "Rubric Successfully Cloned from Block ID: "
@@ -1820,17 +1834,14 @@
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σł#"
 
 msgid "Save"
 msgstr "Sävé Ⱡ'σяєм ι#"
 
-msgid "Save your progress"
-msgstr "Sävé ýöür prögréss Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
-
 msgid "Schedule"
 msgstr "Sçhédülé Ⱡ'σяєм ιρѕυм ∂#"
 
 msgid "Scored Response"
 msgstr "Sçöréd Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
 msgid "Select Team-Set"
@@ -2030,14 +2041,17 @@
 
 msgid "Start Time"
 msgstr "Stärt Tïmé Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
 msgid "Status"
 msgstr "Stätüs Ⱡ'σяєм ιρѕυ#"
 
+msgid "Status of Your Response"
+msgstr "Stätüs öf Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
+
 msgid "Step: Learner Training"
 msgstr "Stép: Léärnér Träïnïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
 msgid "Step: Peer Assessment"
 msgstr "Stép: Péér Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
 msgid "Step: Self Assessment"
@@ -2050,14 +2064,19 @@
 msgstr "Süßmïssïön ÌD Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
 msgid "Submission cannot be empty. Please refresh the page and try again."
 msgstr ""
 "Süßmïssïön çännöt ßé émptý. Pléäsé réfrésh thé pägé änd trý ägäïn. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
+msgid "Submission data missing. Please contact support staff."
+msgstr ""
+"Süßmïssïön dätä mïssïng. Pléäsé çöntäçt süppört stäff. Ⱡ'σяєм ιρѕυм ∂σłσя "
+"ѕιт αмєт, ¢σηѕє¢тєтυя α#"
+
 msgid "Submission for team assignment has no associated team submission"
 msgstr ""
 "Süßmïssïön för téäm ässïgnmént häs nö ässöçïätéd téäm süßmïssïön Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
 msgid "Submission not found"
 msgstr "Süßmïssïön nöt föünd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
@@ -2486,31 +2505,14 @@
 msgstr "Thïs ïs ä téäm süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
 msgid "This problem must include at least one assessment."
 msgstr ""
 "Thïs prößlém müst ïnçlüdé ät léäst öné ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-msgid "This response could not be saved."
-msgstr ""
-"Thïs réspönsé çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
-
-msgid "This response has been saved but not submitted."
-msgstr ""
-"Thïs réspönsé häs ßéén sävéd ßüt nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя α#"
-
-msgid "This response has not been saved."
-msgstr ""
-"Thïs réspönsé häs nöt ßéén sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
-
-msgid "This response was not submitted."
-msgstr ""
-"Thïs réspönsé wäs nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
-
 msgid "This rubric definition is not valid."
 msgstr ""
 "Thïs rüßrïç défïnïtïön ïs nöt välïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
 msgid ""
 "This step's due date '{due}' cannot be later than the next step's due date "
 "'{prev}'."
@@ -2681,20 +2683,14 @@
 msgstr ""
 "Ýöü Müst Çömplété thé Stéps Àßövé tö Vïéw Ýöür Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
 msgid "You are on team "
 msgstr "Ýöü äré ön téäm  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-msgid ""
-"You can save your progress and return to complete your response at any time."
-msgstr ""
-"Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété ýöür réspönsé ät äný tïmé. "
-"Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
-
 msgid "You cannot delete a criterion after the assignment has been released."
 msgstr ""
 "Ýöü çännöt délété ä çrïtérïön äftér thé ässïgnmént häs ßéén réléäséd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
 msgid "You cannot delete a prompt after the assignment has been released."
 msgstr ""
@@ -2788,19 +2784,14 @@
 msgid ""
 "You have successfully completed this problem and received a {earned_points}/"
 "{total_points}."
 msgstr ""
 "Ýöü hävé süççéssfüllý çömplétéd thïs prößlém änd réçéïvéd ä {earned_points}/"
 "{total_points}. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-msgid "You may continue to work on your response until you submit it."
-msgstr ""
-"Ýöü mäý çöntïnüé tö wörk ön ýöür réspönsé üntïl ýöü süßmït ït. Ⱡ'σяєм ιρѕυм "
-"∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
-
 msgid "You must provide at least one example response for learner training."
 msgstr ""
 "Ýöü müst prövïdé ät léäst öné éxämplé réspönsé för léärnér träïnïng. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
 msgid "You must provide feedback for criteria in the assessment."
 msgstr ""
@@ -2843,17 +2834,14 @@
 
 msgid "Your Response "
 msgstr "Ýöür Réspönsé  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
 msgid "Your Self Assessment"
 msgstr "Ýöür Sélf Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-msgid "Your Submission Status"
-msgstr "Ýöür Süßmïssïön Stätüs Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
-
 msgid "Your Team's Response"
 msgstr "Ýöür Téäm's Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
 msgid "Your Upload"
 msgstr "Ýöür Ûplöäd Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
 msgid "Your Uploaded Files"
@@ -2949,14 +2937,21 @@
 "résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
 "єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
 "єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
 "αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
 "νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
 "σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ι#"
 
+msgid ""
+"Your work will save automatically and you can return to complete your "
+"response at any time."
+msgstr ""
+"Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn tö çömplété ýöür "
+"réspönsé ät äný tïmé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
+
 msgid "options_selected must be a dictionary"
 msgstr ""
 "öptïöns_séléçtéd müst ßé ä dïçtïönärý Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
 msgid "points"
 msgstr "pöïnts Ⱡ'σяєм ιρѕυ#"
```

### Comparing `ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/django.po`

 * *Files 17% similar despite different names*

```diff
@@ -4,175 +4,175 @@
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # EdX Team <info@edx.org>, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-ora2\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-09-13 04:00-0400\n"
+"POT-Creation-Date: 2023-06-21 17:18+0000\n"
 "PO-Revision-Date: 2014-06-04 15:41-0400\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
 "Language-Team: openedx-translation <openedx-translation@googlegroups.com>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 msgid "Could not parse serialized rubric"
 msgstr ""
 "Çöüld nöt pärsé sérïälïzéd rüßrïç Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 msgid ""
 "If your assignment includes a learner training step, the rubric must have at"
 " least one criterion, and that criterion must have at least one option."
 msgstr ""
 "Ìf ýöür ässïgnmént ïnçlüdés ä léärnér träïnïng stép, thé rüßrïç müst hävé ät"
 " léäst öné çrïtérïön, änd thät çrïtérïön müst hävé ät léäst öné öptïön. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
 "тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
 " qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм #"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 #, python-brace-format
 msgid "Example {example_number} has a validation error: {error}"
 msgstr ""
 "Éxämplé {example_number} häs ä välïdätïön érrör: {error} Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 #, python-brace-format
 msgid ""
 "Example {example_number} has an invalid option for \"{criterion_name}\": "
 "\"{option_name}\""
 msgstr ""
 "Éxämplé {example_number} häs än ïnvälïd öptïön för \"{criterion_name}\": "
 "\"{option_name}\" Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 #, python-brace-format
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
 msgstr ""
 "Éxämplé {example_number} häs än éxträ öptïön för \"{criterion_name}\" Ⱡ'σяєм"
 " ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/assessment/api/student_training.py
+#: assessment/api/student_training.py
 #, python-brace-format
 msgid "Example {example_number} is missing an option for \"{criterion_name}\""
 msgstr ""
 "Éxämplé {example_number} ïs mïssïng än öptïön för \"{criterion_name}\" "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/data.py
+#: data.py
 #, python-brace-format
 msgid "Criterion {number}: {label}"
 msgstr "Çrïtérïön {number}: {label} Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/data.py
+#: data.py
 #, python-brace-format
 msgid "Points {number}"
 msgstr "Pöïnts {number} Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/data.py
+#: data.py
 #, python-brace-format
 msgid "Median Score {number}"
 msgstr "Médïän Sçöré {number} Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/data.py
+#: data.py
 #, python-brace-format
 msgid "Feedback {number}"
 msgstr "Féédßäçk {number} Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Item ID"
 msgstr "Ìtém ÌD Ⱡ'σяєм ιρѕυм #"
 
-#: openassessment/data.py
+#: data.py
 msgid "Submission ID"
 msgstr "Süßmïssïön ÌD Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Anonymized Student ID"
 msgstr "Ànönýmïzéd Stüdént ÌD Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment ID"
 msgstr "Àsséssmént ÌD Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment Scored Date"
 msgstr "Àsséssmént Sçöréd Däté Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment Scored Time"
 msgstr "Àsséssmént Sçöréd Tïmé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment Type"
 msgstr "Àsséssmént Týpé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Anonymous Scorer Id"
 msgstr "Ànönýmöüs Sçörér Ìd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/data.py
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: data.py
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Overall Feedback"
 msgstr "Övéräll Féédßäçk Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment Score Earned"
 msgstr "Àsséssmént Sçöré Éärnéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Assessment Scored At"
 msgstr "Àsséssmént Sçöréd Àt Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/data.py
+#: data.py
 msgid "Date/Time Final Score Given"
 msgstr "Däté/Tïmé Fïnäl Sçöré Gïvén Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Final Score Earned"
 msgstr "Fïnäl Sçöré Éärnéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Final Score Possible"
 msgstr "Fïnäl Sçöré Pössïßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/data.py
+#: data.py
 msgid "Feedback Statements Selected"
 msgstr "Féédßäçk Stätéménts Séléçtéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Feedback on Assessment"
 msgstr "Féédßäçk ön Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/data.py
+#: data.py
 msgid "Response Files"
 msgstr "Réspönsé Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/data.py
+#: data.py
 msgid "No description provided."
 msgstr "Nö désçrïptïön prövïdéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit.html
+#: templates/openassessmentblock/edit/oa_edit.html
 msgid "Save"
 msgstr "Sävé Ⱡ'σяєм ι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit.html
+#: templates/openassessmentblock/edit/oa_edit.html
 msgid "Cancel"
 msgstr "Çänçél Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
+#: templates/openassessmentblock/edit/oa_edit_assessment_steps.html
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
 msgstr ""
 "Öpén Réspönsé Àsséssménts ällöw ýöü tö çönfïgüré sïnglé ör mültïplé stéps ïn"
@@ -180,438 +180,438 @@
 " çän ßé énäßléd, dïsäßlé, änd ördéréd för ä fléxïßlé sét öf pédägögïçäl "
 "nééds. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ "
 "єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм"
 " νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα "
 "¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт"
 " єѕѕє ¢ιłłυм ∂σłσяє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Display Name "
 msgstr "Dïspläý Nämé  Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "The display name for this component."
 msgstr ""
 "Thé dïspläý nämé för thïs çömpönént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Text Response"
 msgstr "Téxt Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify whether learners must include a text based response to this "
 "problem's prompt."
 msgstr ""
 "Spéçïfý whéthér léärnérs müst ïnçlüdé ä téxt ßäséd réspönsé tö thïs "
 "prößlém's prömpt. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Response Editor"
 msgstr "Réspönsé Édïtör Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Select which editor learners will use to include a text based response to "
 "this problem's prompt."
 msgstr ""
 "Séléçt whïçh édïtör léärnérs wïll üsé tö ïnçlüdé ä téxt ßäséd réspönsé tö "
 "thïs prößlém's prömpt. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "File Uploads Response"
 msgstr "Fïlé Ûplöäds Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify whether learners are able to upload files as a part of their "
 "response."
 msgstr ""
 "Spéçïfý whéthér léärnérs äré äßlé tö üplöäd fïlés äs ä pärt öf théïr "
 "réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Allow Multiple Files"
 msgstr "Àllöw Mültïplé Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "False"
 msgstr "Fälsé Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "True"
 msgstr "Trüé Ⱡ'σяєм ι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
 "Spéçïfý whéthér léärnérs çän üplöäd möré thän öné fïlé. Thïs häs nö éfféçt "
 "ïf Fïlé Ûplöäds Réspönsé ïs sét tö Nöné. Thïs ïs äütömätïçällý sét tö Trüé "
 "för Téäm Àssïgnménts.  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
 "єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
 "єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
 "αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
 "νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
 "σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "File Upload Types"
 msgstr "Fïlé Ûplöäd Týpés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "PDF or Image Files"
 msgstr "PDF ör Ìmägé Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Image Files"
 msgstr "Ìmägé Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Custom File Types"
 msgstr "Çüstöm Fïlé Týpés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify whether learners can submit files along with their text responses."
 msgstr ""
 "Spéçïfý whéthér léärnérs çän süßmït fïlés älöng wïth théïr téxt réspönsés. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "File Types"
 msgstr "Fïlé Týpés Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Enter the file extensions, separated by commas, that you want learners to be"
 " able to upload. For example: pdf,doc,docx."
 msgstr ""
 "Éntér thé fïlé éxténsïöns, sépärätéd ßý çömmäs, thät ýöü wänt léärnérs tö ßé"
 " äßlé tö üplöäd. För éxämplé: pdf,döç,döçx. Ⱡ'σяєм ιρѕυм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "To add more file extensions, select Custom File Types and enter the full "
 "list of acceptable file extensions to be included."
 msgstr ""
 "Tö ädd möré fïlé éxténsïöns, séléçt Çüstöm Fïlé Týpés änd éntér thé füll "
 "lïst öf äççéptäßlé fïlé éxténsïöns tö ßé ïnçlüdéd. Ⱡ'σяєм ιρ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Allow LaTeX Responses"
 msgstr "Àllöw LäTéX Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Specify whether learners can write LaTeX formatted strings"
 msgstr ""
 "Spéçïfý whéthér léärnérs çän wrïté LäTéX förmättéd strïngs Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
-#: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
-#: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+#: templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
 msgid "Top Responses"
 msgstr "Töp Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid " (Disabled)"
 msgstr " (Dïsäßléd) Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify the number of top scoring responses to display after the learner has"
 " submitted a response. Valid numbers are 0 to 99. If the number is 0, the "
 "Top Responses section does not appear to learners."
 msgstr ""
 "Spéçïfý thé nümßér öf töp sçörïng réspönsés tö dïspläý äftér thé léärnér häs"
 " süßmïttéd ä réspönsé. Välïd nümßérs äré 0 tö 99. Ìf thé nümßér ïs 0, thé "
 "Töp Réspönsés séçtïön döés nöt äppéär tö léärnérs. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт "
 "łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ "
 "єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ "
 "αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ "
 "ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "When Teams Enabled is set to true, Top Responses will be disabled."
 msgstr ""
 "Whén Téäms Énäßléd ïs sét tö trüé, Töp Réspönsés wïll ßé dïsäßléd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Teams Enabled"
 msgstr "Téäms Énäßléd Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Specify whether team submissions are allowed for this response."
 msgstr ""
 "Spéçïfý whéthér téäm süßmïssïöns äré ällöwéd för thïs réspönsé. Ⱡ'σяєм ιρѕυм"
 " ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Select Team-Set"
 msgstr "Séléçt Téäm-Sét Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid "Show Rubric During Response"
 msgstr "Shöw Rüßrïç Dürïng Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+#: templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
 msgid ""
 "Specify whether learners can see the rubric while they are working on their "
 "response."
 msgstr ""
 "Spéçïfý whéthér léärnérs çän séé thé rüßrïç whïlé théý äré wörkïng ön théïr "
 "réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Criterion"
 msgstr "Çrïtérïön Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid "You cannot delete a criterion after the assignment has been released."
 msgstr ""
 "Ýöü çännöt délété ä çrïtérïön äftér thé ässïgnmént häs ßéén réléäséd. Ⱡ'σяєм"
 " ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_option.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
-#: openassessment/templates/openassessmentblock/edit/oa_training_example.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_option.html
+#: templates/openassessmentblock/edit/oa_edit_prompt.html
+#: templates/openassessmentblock/edit/oa_training_example.html
 msgid "Remove"
 msgstr "Rémövé Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid "Criterion Name"
 msgstr "Çrïtérïön Nämé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid "Criterion Prompt"
 msgstr "Çrïtérïön Prömpt Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid "Add Option"
 msgstr "Àdd Öptïön Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid "Feedback for This Criterion"
 msgstr "Féédßäçk för Thïs Çrïtérïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
-#: openassessment/xblock/studio_mixin.py
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
+#: xblock/studio_mixin.py
 msgid "None"
 msgstr "Nöné Ⱡ'σяєм ι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
-#: openassessment/xblock/studio_mixin.py
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
+#: xblock/studio_mixin.py
 msgid "Optional"
 msgstr "Öptïönäl Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
-#: openassessment/templates/openassessmentblock/oa_rubric.html
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
-#: openassessment/xblock/studio_mixin.py
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/oa_rubric.html
+#: templates/openassessmentblock/student_training/student_training.html
+#: xblock/studio_mixin.py
 msgid "Required"
 msgstr "Réqüïréd Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+#: templates/openassessmentblock/edit/oa_edit_criterion.html
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 "Séléçt öné öf thé öptïöns äßövé. Thïs désçrïßés whéthér ör nöt thé révïéwér "
 "wïll hävé tö prövïdé çrïtérïön féédßäçk. Ⱡ'σяєм ιρѕυм ∂σ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
 msgid "Open Response Assessment"
 msgstr "Öpén Réspönsé Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_prompt.html
 msgid "Prompt"
 msgstr "Prömpt Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
 msgid "Rubric"
 msgstr "Rüßrïç Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
 msgid "Schedule"
 msgstr "Sçhédülé Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
 msgid "Assessment steps"
 msgstr "Àsséssmént stéps Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+#: templates/openassessmentblock/edit/oa_edit_header_and_validation.html
 msgid "Settings"
 msgstr "Séttïngs Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+#: templates/openassessmentblock/edit/oa_edit_option.html
 msgid "Option"
 msgstr "Öptïön Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+#: templates/openassessmentblock/edit/oa_edit_option.html
 msgid "Option Name"
 msgstr "Öptïön Nämé Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+#: templates/openassessmentblock/edit/oa_edit_option.html
 msgid "Option Points"
 msgstr "Öptïön Pöïnts Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+#: templates/openassessmentblock/edit/oa_edit_option.html
 msgid "Option Explanation"
 msgstr "Öptïön Éxplänätïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "Step: Peer Assessment"
 msgstr "Stép: Péér Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid ""
 "Peer Assessment allows students to provide feedback to other students and "
 "also receive feedback from others in their final grade. Often, though not "
 "always, this step is preceded by Self Assessment or Learner Training steps."
 msgstr ""
 "Péér Àsséssmént ällöws stüdénts tö prövïdé féédßäçk tö öthér stüdénts änd "
 "älsö réçéïvé féédßäçk fröm öthérs ïn théïr fïnäl grädé. Öftén, thöügh nöt "
 "älwäýs, thïs stép ïs préçédéd ßý Sélf Àsséssmént ör Léärnér Träïnïng stéps. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
 "тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
 " qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid ""
 "Configuration: For this step to be configured you must specify the number of"
 " peer reviews a student will be assessed with, and the number of peer a "
 "student must grade. Additional options can be specified."
 msgstr ""
 "Çönfïgürätïön: För thïs stép tö ßé çönfïgüréd ýöü müst spéçïfý thé nümßér öf"
 " péér révïéws ä stüdént wïll ßé ässésséd wïth, änd thé nümßér öf péér ä "
 "stüdént müst grädé. Àddïtïönäl öptïöns çän ßé spéçïfïéd. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт "
 "łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ "
 "єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ "
 "αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ "
 "ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "View Options & Configuration"
 msgstr "Vïéw Öptïöns & Çönfïgürätïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "Must Grade"
 msgstr "Müst Grädé Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid ""
 "Specify the number of peer assessments that each learner must complete. "
 "Valid numbers are 1 to 99."
 msgstr ""
 "Spéçïfý thé nümßér öf péér ässéssménts thät éäçh léärnér müst çömplété. "
 "Välïd nümßérs äré 1 tö 99. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "Graded By"
 msgstr "Grädéd Bý Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid ""
 "Specify the number of learners that each response must be assessed by. Valid"
 " numbers are 1 to 99."
 msgstr ""
 "Spéçïfý thé nümßér öf léärnérs thät éäçh réspönsé müst ßé ässésséd ßý. Välïd"
 " nümßérs äré 1 tö 99. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 msgid "Enable Flexible Peer Grade Averaging"
 msgstr ""
 "Énäßlé Fléxïßlé Péér Grädé Àvérägïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment.html
 #, python-format
 msgid ""
 "When enabled, learners who have received at least 30%% of the required \\"
 msgstr ""
 "Whén énäßléd, léärnérs whö hävé réçéïvéd ät léäst 30%% öf thé réqüïréd \\ "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
 msgid "Peer Assessment Deadlines"
 msgstr "Péér Àsséssmént Déädlïnés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "Start Date"
 msgstr "Stärt Däté Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "Start Time"
 msgstr "Stärt Tïmé Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 "Thé däté änd tïmé whén léärnérs çän ßégïn ässéssïng péér réspönsés. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Due Date"
 msgstr "Düé Däté Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "Due Time"
 msgstr "Düé Tïmé Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
 msgid "The date and time when all peer assessments must be complete."
 msgstr ""
 "Thé däté änd tïmé whén äll péér ässéssménts müst ßé çömplété. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+#: templates/openassessmentblock/edit/oa_edit_prompt.html
 msgid "You cannot delete a prompt after the assignment has been released."
 msgstr ""
 "Ýöü çännöt délété ä prömpt äftér thé ässïgnmént häs ßéén réléäséd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+#: templates/openassessmentblock/edit/oa_edit_prompts.html
 msgid ""
 "Prompts. Replace the sample text with your own text. For more information, "
 "see the ORA documentation."
 msgstr ""
 "Prömpts. Répläçé thé sämplé téxt wïth ýöür öwn téxt. För möré ïnförmätïön, "
 "séé thé ÖRÀ döçüméntätïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+#: templates/openassessmentblock/edit/oa_edit_prompts.html
 msgid "Add Prompt"
 msgstr "Àdd Prömpt Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid ""
 "Rubrics are made up of criteria, which usually contain one or more options. "
 "Each option has a point value. This template contains two sample criteria "
 "and their options. Replace the sample text with your own text. For more "
 "information, see the ORA documentation."
 msgstr ""
 "Rüßrïçs äré mädé üp öf çrïtérïä, whïçh üsüällý çöntäïn öné ör möré öptïöns. "
@@ -619,150 +619,150 @@
 "änd théïr öptïöns. Répläçé thé sämplé téxt wïth ýöür öwn téxt. För möré "
 "ïnförmätïön, séé thé ÖRÀ döçüméntätïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σł#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid "Add Criterion"
 msgstr "Àdd Çrïtérïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid "Feedback for This Response"
 msgstr "Féédßäçk för Thïs Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid "Feedback Instructions"
 msgstr "Féédßäçk Ìnstrüçtïöns Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid ""
 "Encourage learners to provide feedback on the response they have graded. You"
 " can replace the sample text with your own."
 msgstr ""
 "Énçöürägé léärnérs tö prövïdé féédßäçk ön thé réspönsé théý hävé grädéd. Ýöü"
 " çän répläçé thé sämplé téxt wïth ýöür öwn. Ⱡ'σяєм ιρѕυм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid "Default Feedback Text"
 msgstr "Défäült Féédßäçk Téxt Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+#: templates/openassessmentblock/edit/oa_edit_rubric.html
 msgid ""
 "Enter feedback text that learners will see before they enter their own "
 "feedback. Use this text to show learners a good example peer assessment."
 msgstr ""
 "Éntér féédßäçk téxt thät léärnérs wïll séé ßéföré théý éntér théïr öwn "
 "féédßäçk. Ûsé thïs téxt tö shöw léärnérs ä gööd éxämplé péér ässéssmént. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
 "тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
 " qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "Course Deadlines"
 msgstr "Çöürsé Déädlïnés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "Response Start Date"
 msgstr "Réspönsé Stärt Däté Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "Response Start Time"
 msgstr "Réspönsé Stärt Tïmé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "The date and time when learners can begin submitting responses."
 msgstr ""
 "Thé däté änd tïmé whén léärnérs çän ßégïn süßmïttïng réspönsés. Ⱡ'σяєм ιρѕυм"
 " ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "Response Due Date"
 msgstr "Réspönsé Düé Däté Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "Response Due Time"
 msgstr "Réspönsé Düé Tïmé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_schedule.html
 msgid "The date and time when learners can no longer submit responses."
 msgstr ""
 "Thé däté änd tïmé whén léärnérs çän nö löngér süßmït réspönsés. Ⱡ'σяєм ιρѕυм"
 " ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment.html
 msgid "Step: Self Assessment"
 msgstr "Stép: Sélf Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment.html
 msgid ""
 "Self Assessment asks learners to grade their own submissions against the "
 "rubric."
 msgstr ""
 "Sélf Àsséssmént äsks léärnérs tö grädé théïr öwn süßmïssïöns ägäïnst thé "
 "rüßrïç. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "Self Assessment Deadlines"
 msgstr "Sélf Àsséssmént Déädlïnés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "The date and time when learners can begin assessing their responses."
 msgstr ""
 "Thé däté änd tïmé whén léärnérs çän ßégïn ässéssïng théïr réspönsés. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+#: templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
 msgid "The date and time when all self assessments must be complete."
 msgstr ""
 "Thé däté änd tïmé whén äll sélf ässéssménts müst ßé çömplété. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_staff_assessment.html
 msgid "Step: Staff Assessment"
 msgstr "Stép: Stäff Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+#: templates/openassessmentblock/edit/oa_edit_staff_assessment.html
 msgid ""
 "Staff Assessment gates sets the final grade for students if enabled with "
 "other steps, though it can also be used as a standalone step."
 msgstr ""
 "Stäff Àsséssmént gätés séts thé fïnäl grädé för stüdénts ïf énäßléd wïth "
 "öthér stéps, thöügh ït çän älsö ßé üséd äs ä ständälöné stép. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт łαвσяυм#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+#: templates/openassessmentblock/edit/oa_edit_student_training.html
 msgid "Step: Learner Training"
 msgstr "Stép: Léärnér Träïnïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+#: templates/openassessmentblock/edit/oa_edit_student_training.html
 msgid ""
 "Learner Training is used to help students practice grading a simulated peer "
 "submission in order to train them on the rubric and ensure learner's "
 "understand the rubric for either Self or Peer Assessment steps."
 msgstr ""
 "Léärnér Träïnïng ïs üséd tö hélp stüdénts präçtïçé grädïng ä sïmülätéd péér "
 "süßmïssïön ïn ördér tö träïn thém ön thé rüßrïç änd énsüré léärnér's "
 "ündérständ thé rüßrïç för éïthér Sélf ör Péér Àsséssmént stéps. Ⱡ'σяєм ιρѕυм"
 " ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+#: templates/openassessmentblock/edit/oa_edit_student_training.html
 msgid ""
 "Configuration: For this step to be fully configured you must provide one or "
 "more graded sample responses. Learners must then match this instructor score"
 " to advance and are provided feedback when their score doesn't match the "
 "sample response."
 msgstr ""
 "Çönfïgürätïön: För thïs stép tö ßé füllý çönfïgüréd ýöü müst prövïdé öné ör "
@@ -770,27 +770,27 @@
 " tö ädvänçé änd äré prövïdéd féédßäçk whén théïr sçöré döésn't mätçh thé "
 "sämplé réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, "
 "ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм "
 "α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ "
 "єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє"
 " νєłιт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+#: templates/openassessmentblock/edit/oa_edit_student_training.html
 msgid "View / Add Sample Responses"
 msgstr "Vïéw / Àdd Sämplé Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+#: templates/openassessmentblock/edit/oa_edit_student_training.html
 msgid "Add Sample Response"
 msgstr "Àdd Sämplé Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "Clone Rubric"
 msgstr "Çlöné Rüßrïç Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid ""
 "To clone a rubric from an existing published or unpublished draft, you can "
 "search by the Block ID. Note that cloning is one-way, meaning changes made "
 "after cloning will only affect the rubric being modified, and will not "
 "modify any rubric it was cloned from."
 msgstr ""
 "Tö çlöné ä rüßrïç fröm än éxïstïng püßlïshéd ör ünpüßlïshéd dräft, ýöü çän "
@@ -798,72 +798,72 @@
 "äftér çlönïng wïll önlý äfféçt thé rüßrïç ßéïng mödïfïéd, änd wïll nöt "
 "mödïfý äný rüßrïç ït wäs çlönéd fröm. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "Block ID For this ORA:"
 msgstr "Blöçk ÌD För thïs ÖRÀ: Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "Block ID"
 msgstr "Blöçk ÌD Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "No other Open Response Assessments found in course"
 msgstr ""
 "Nö öthér Öpén Réspönsé Àsséssménts föünd ïn çöürsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "Clone"
 msgstr "Çlöné Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+#: templates/openassessmentblock/edit/oa_rubric_reuse.html
 msgid "Rubric Successfully Cloned from Block ID: "
 msgstr ""
 "Rüßrïç Süççéssfüllý Çlönéd fröm Blöçk ÌD:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/edit/oa_training_example.html
+#: templates/openassessmentblock/edit/oa_training_example.html
 msgid "Scored Response"
 msgstr "Sçöréd Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_training_example.html
+#: templates/openassessmentblock/edit/oa_training_example.html
 msgid "Response Score"
 msgstr "Réspönsé Sçöré Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_training_example.html
+#: templates/openassessmentblock/edit/oa_training_example.html
 msgid "Response"
 msgstr "Réspönsé Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
+#: templates/openassessmentblock/edit/oa_training_example_criterion.html
 msgid "Not Selected"
 msgstr "Nöt Séléçtéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
-#: openassessment/templates/openassessmentblock/oa_rubric.html
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/edit/oa_training_example_criterion.html
+#: templates/openassessmentblock/oa_rubric.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "points"
 msgstr "pöïnts Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
+#: templates/openassessmentblock/grade/oa_assessment_feedback.html
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
 msgstr ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "               Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+#: templates/openassessmentblock/grade/oa_assessment_title.html
 #, python-format
 msgid ""
 "\n"
 "                      %(assessment_title)s - %(points)s point\n"
 "                  "
 msgid_plural ""
 "\n"
@@ -874,737 +874,736 @@
 "                      %(assessment_title)s - %(points)s pöïnt\n"
 "                   Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 msgstr[1] ""
 "\n"
 "                      %(assessment_title)s - %(points)s pöïnts\n"
 "                   Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+#: templates/openassessmentblock/grade/oa_assessment_title.html
 #, python-format
 msgid "More information about %(name)s"
 msgstr "Möré ïnförmätïön äßöüt %(name)s Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+#: templates/openassessmentblock/grade/oa_grade_cancelled.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_incomplete.html
+#: templates/openassessmentblock/grade/oa_grade_not_started.html
+#: templates/openassessmentblock/grade/oa_grade_waiting.html
 msgid "Your Grade"
 msgstr "Ýöür Grädé Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+#: templates/openassessmentblock/grade/oa_grade_cancelled.html
 #, python-format
 msgid ""
 "\n"
 "                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
 msgstr ""
 "\n"
 "                                        %(points_earned)s öüt öf %(points_possible)s\n"
 "                                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+#: templates/openassessmentblock/grade/oa_grade_cancelled.html
 msgid "Your submission has been cancelled."
 msgstr ""
 "Ýöür süßmïssïön häs ßéén çänçélléd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 #, python-format
 msgid ""
 "\n"
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 "\n"
 "                                            %(points_earned)s öüt öf %(points_possible)s\n"
 "                                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Your Response"
 msgstr "Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Your Upload"
 msgstr "Ýöür Ûplöäd Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Assessments of Your Response"
 msgstr "Àsséssménts öf Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
-#: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
-#: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
-#: openassessment/templates/openassessmentblock/message/oa_message_closed.html
-#: openassessment/templates/openassessmentblock/message/oa_message_complete.html
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
-#: openassessment/templates/openassessmentblock/response/oa_response_closed.html
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
-#: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
-#: openassessment/templates/openassessmentblock/self/oa_self_closed.html
-#: openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_incomplete.html
+#: templates/openassessmentblock/grade/oa_grade_waiting.html
+#: templates/openassessmentblock/message/oa_message_cancelled.html
+#: templates/openassessmentblock/message/oa_message_closed.html
+#: templates/openassessmentblock/message/oa_message_complete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/peer/oa_peer_closed.html
+#: templates/openassessmentblock/peer/oa_peer_complete.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_waiting.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/response/oa_response_closed.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_team_already_submitted.html
+#: templates/openassessmentblock/self/oa_self_closed.html
+#: templates/openassessmentblock/student_training/student_training_closed.html
 msgid "Status"
 msgstr "Stätüs Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Overall Grade"
 msgstr "Övéräll Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Points"
 msgstr "Pöïnts Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Additional comments on your response"
 msgstr ""
 "Àddïtïönäl çömménts ön ýöür réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Provide feedback on peer assessments"
 msgstr ""
 "Prövïdé féédßäçk ön péér ässéssménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Submitting Feedback"
 msgstr "Süßmïttïng Féédßäçk Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid ""
 "Your feedback has been submitted. Course staff will be able to see this "
 "feedback when they review course records."
 msgstr ""
 "Ýöür féédßäçk häs ßéén süßmïttéd. Çöürsé stäff wïll ßé äßlé tö séé thïs "
 "féédßäçk whén théý révïéw çöürsé réçörds. Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid ""
 "Course staff will be able to see any feedback that you provide here when "
 "they review course records."
 msgstr ""
 "Çöürsé stäff wïll ßé äßlé tö séé äný féédßäçk thät ýöü prövïdé héré whén "
 "théý révïéw çöürsé réçörds. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid ""
 "Select the statements below that best reflect your experience with peer "
 "assessments."
 msgstr ""
 "Séléçt thé stätéménts ßélöw thät ßést réfléçt ýöür éxpérïénçé wïth péér "
 "ässéssménts. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "These assessments were useful."
 msgstr "Thésé ässéssménts wéré üséfül. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "These assessments were not useful."
 msgstr ""
 "Thésé ässéssménts wéré nöt üséfül. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "I disagree with one or more of the peer assessments of my response."
 msgstr ""
 "Ì dïsägréé wïth öné ör möré öf thé péér ässéssménts öf mý réspönsé. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Some comments I received were inappropriate."
 msgstr ""
 "Sömé çömménts Ì réçéïvéd wéré ïnäppröprïäté. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid ""
 "Provide feedback on the grade or comments that you received from your peers."
 msgstr ""
 "Prövïdé féédßäçk ön thé grädé ör çömménts thät ýöü réçéïvéd fröm ýöür péérs."
 " Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "I feel the feedback I received was..."
 msgstr ""
 "Ì féél thé féédßäçk Ì réçéïvéd wäs... Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "We could not submit your feedback"
 msgstr ""
 "Wé çöüld nöt süßmït ýöür féédßäçk Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+#: templates/openassessmentblock/grade/oa_grade_complete.html
 msgid "Submit feedback on peer assessments"
 msgstr ""
 "Süßmït féédßäçk ön péér ässéssménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+#: templates/openassessmentblock/grade/oa_grade_incomplete.html
 msgid "Not Completed"
 msgstr "Nöt Çömplétéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+#: templates/openassessmentblock/grade/oa_grade_incomplete.html
 msgid "You have not completed all the steps of this problem."
 msgstr ""
 "Ýöü hävé nöt çömplétéd äll thé stéps öf thïs prößlém. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт"
 " αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+#: templates/openassessmentblock/grade/oa_grade_not_started.html
 msgid "Not Started"
 msgstr "Nöt Stärtéd Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+#: templates/openassessmentblock/grade/oa_grade_not_started.html
 msgid "You have not started this problem yet."
 msgstr ""
 "Ýöü hävé nöt stärtéd thïs prößlém ýét. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+#: templates/openassessmentblock/grade/oa_grade_waiting.html
 msgid "Waiting for Assessments"
 msgstr "Wäïtïng för Àsséssménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
-#: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+#: templates/openassessmentblock/grade/oa_grade_waiting.html
 msgid ""
 "You have completed your steps in the assignment, but some assessments still "
 "need to be done on your response. When the assessments of your response are "
 "complete, you will see feedback from everyone who assessed your response, "
 "and you will receive your final grade."
 msgstr ""
 "Ýöü hävé çömplétéd ýöür stéps ïn thé ässïgnmént, ßüt sömé ässéssménts stïll "
 "nééd tö ßé döné ön ýöür réspönsé. Whén thé ässéssménts öf ýöür réspönsé äré "
 "çömplété, ýöü wïll séé féédßäçk fröm évérýöné whö ässésséd ýöür réspönsé, "
 "änd ýöü wïll réçéïvé ýöür fïnäl grädé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυ#"
 
-#: openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Grade Available Responses"
 msgstr "Grädé Àväïläßlé Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+#: templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
 msgid ""
 "Grade Available Responses is unavailable. This item is not configured for "
 "Staff Assessment."
 msgstr ""
 "Grädé Àväïläßlé Réspönsés ïs ünäväïläßlé. Thïs ïtém ïs nöt çönfïgüréd för "
 "Stäff Àsséssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
+#: templates/openassessmentblock/instructor_dashboard/oa_listing.html
 msgid "Please wait"
 msgstr "Pléäsé wäït Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+#: templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
 msgid "Waiting Step Details"
 msgstr "Wäïtïng Stép Détäïls Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+#: templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
 msgid ""
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
 msgstr ""
 "Wäïtïng Stép détäïls vïéw ïs ünäväïläßlé. Thïs ïtém ïs nöt çönfïgüréd för "
 "péér ässéssménts. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+#: templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
 #, python-format
 msgid "%(num_points)s points"
 msgstr "%(num_points)s pöïnts Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
 msgid "Your peer's response to the prompt above"
 msgstr ""
 "Ýöür péér's réspönsé tö thé prömpt äßövé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+#: templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
 msgid ""
 "After you complete all the steps of this assignment, you can see the top-"
 "scoring responses from your peers."
 msgstr ""
 "Àftér ýöü çömplété äll thé stéps öf thïs ässïgnmént, ýöü çän séé thé töp-"
 "sçörïng réspönsés fröm ýöür péérs. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+#: templates/openassessmentblock/message/oa_message_cancelled.html
 msgid ""
 "Your team’s submission has been cancelled. Your team will receive a grade of"
 " zero unless course staff resets your assessment to allow the team to "
 "resubmit a response."
 msgstr ""
 "Ýöür téäm’s süßmïssïön häs ßéén çänçélléd. Ýöür téäm wïll réçéïvé ä grädé öf"
 " zérö ünléss çöürsé stäff réséts ýöür ässéssmént tö ällöw thé téäm tö "
 "résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg "
 "єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт "
 "єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
 "αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
 "νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
 "σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ι#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+#: templates/openassessmentblock/message/oa_message_cancelled.html
 msgid ""
 "Your submission has been cancelled. You will receive a grade of zero unless "
 "course staff resets your assessment to allow you to resubmit a response."
 msgstr ""
 "Ýöür süßmïssïön häs ßéén çänçélléd. Ýöü wïll réçéïvé ä grädé öf zérö ünléss "
 "çöürsé stäff réséts ýöür ässéssmént tö ällöw ýöü tö résüßmït ä réspönsé. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
 "тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
 " qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_closed.html
+#: templates/openassessmentblock/message/oa_message_closed.html
 msgid ""
 "This task is not yet available. Check back to complete the assignment once "
 "this section has opened."
 msgstr ""
 "Thïs täsk ïs nöt ýét äväïläßlé. Çhéçk ßäçk tö çömplété thé ässïgnmént önçé "
 "thïs séçtïön häs öpénéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_closed.html
+#: templates/openassessmentblock/message/oa_message_closed.html
 msgid ""
 "This assignment has closed. One or more deadlines for this assignment have "
 "passed. You will receive an incomplete grade for this assignment."
 msgstr ""
 "Thïs ässïgnmént häs çlöséd. Öné ör möré déädlïnés för thïs ässïgnmént hävé "
 "pässéd. Ýöü wïll réçéïvé än ïnçömplété grädé för thïs ässïgnmént. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт ł#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_complete.html
+#: templates/openassessmentblock/message/oa_message_complete.html
 msgid ""
 "You have completed this assignment. Your final grade will be available when "
 "the assessments of your response are complete."
 msgstr ""
 "Ýöü hävé çömplétéd thïs ässïgnmént. Ýöür fïnäl grädé wïll ßé äväïläßlé whén "
 "thé ässéssménts öf ýöür réspönsé äré çömplété. Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_complete.html
+#: templates/openassessmentblock/message/oa_message_complete.html
 msgid ""
 "You have completed this assignment. Review your grade and your assessment "
 "details."
 msgstr ""
 "Ýöü hävé çömplétéd thïs ässïgnmént. Révïéw ýöür grädé änd ýöür ässéssmént "
 "détäïls. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 msgid ""
 "This assignment is in progress. Learner training will close soon. Complete "
 "the learner training step to move on."
 msgstr ""
 "Thïs ässïgnmént ïs ïn prögréss. Léärnér träïnïng wïll çlösé söön. Çömplété "
 "thé léärnér träïnïng stép tö mövé ön. Ⱡ'σяєм ιρѕυм ∂σłσя#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 msgid ""
 "This assignment is in progress. Complete the learner training step to move "
 "on."
 msgstr ""
 "Thïs ässïgnmént ïs ïn prögréss. Çömplété thé léärnér träïnïng stép tö mövé "
 "ön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 msgid ""
 "This assignment is in progress. Check back later when the assessment period "
 "has started."
 msgstr ""
 "Thïs ässïgnmént ïs ïn prögréss. Çhéçk ßäçk lätér whén thé ässéssmént pérïöd "
 "häs stärtéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    %(start_strong)sThis assignment is in progress. The self assessment step will close soon.%(end_strong)s You still need to complete the %(start_link)sself assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    %(start_strong)sThïs ässïgnmént ïs ïn prögréss. Thé sélf ässéssmént stép wïll çlösé söön.%(end_strong)s Ýöü stïll nééd tö çömplété thé %(start_link)ssélf ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    This assignment is in progress. You still need to complete the %(start_link)sself assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    Thïs ässïgnmént ïs ïn prögréss. Ýöü stïll nééd tö çömplété thé %(start_link)ssélf ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    This assignment is in progress.%(start_strong)sThe peer assessment step will close soon.%(end_strong)s All submitted peer responses have been assessed. Check back later to see if more learners have submitted responses. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    Thïs ässïgnmént ïs ïn prögréss.%(start_strong)sThé péér ässéssmént stép wïll çlösé söön.%(end_strong)s Àll süßmïttéd péér réspönsés hävé ßéén ässésséd. Çhéçk ßäçk lätér tö séé ïf möré léärnérs hävé süßmïttéd réspönsés. Ýöü stïll nééd tö çömplété thé %(start_link)spéér ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιq#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    This assignment is in progress. All submitted peer responses have been assessed. Check back later to see if more learners have submitted responses. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    Thïs ässïgnmént ïs ïn prögréss. Àll süßmïttéd péér réspönsés hävé ßéén ässésséd. Çhéçk ßäçk lätér tö séé ïf möré léärnérs hävé süßmïttéd réspönsés. Ýöü stïll nééd tö çömplété thé %(start_link)spéér ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ #"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    This assignment is in progress. %(start_strong)sThe peer assessment step will close soon.%(end_strong)s You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    Thïs ässïgnmént ïs ïn prögréss. %(start_strong)sThé péér ässéssmént stép wïll çlösé söön.%(end_strong)s Ýöü stïll nééd tö çömplété thé %(start_link)spéér ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+#: templates/openassessmentblock/message/oa_message_incomplete.html
 #, python-format
 msgid ""
 "\n"
 "                                    This assignment is in progress. You still need to complete the %(start_link)speer assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    Thïs ässïgnmént ïs ïn prögréss. Ýöü stïll nééd tö çömplété thé %(start_link)spéér ässéssmént%(end_link)s stép.\n"
 "                                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+#: templates/openassessmentblock/message/oa_message_no_team.html
 msgid "Team membership is required to view this assignment"
 msgstr ""
 "Téäm mémßérshïp ïs réqüïréd tö vïéw thïs ässïgnmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+#: templates/openassessmentblock/message/oa_message_no_team.html
 #, python-format
 msgid ""
 "\n"
 "            This is a team assignment for team-set \"%(teamset_name)s\".\n"
 "            You are currently not on a team in team-set \"%(teamset_name)s\".\n"
 "            You must be on a team in team-set \"%(teamset_name)s\" to access this team assignment.\n"
 "            "
 msgstr ""
 "\n"
 "            Thïs ïs ä téäm ässïgnmént för téäm-sét \"%(teamset_name)s\".\n"
 "            Ýöü äré çürréntlý nöt ön ä téäm ïn téäm-sét \"%(teamset_name)s\".\n"
 "            Ýöü müst ßé ön ä téäm ïn téäm-sét \"%(teamset_name)s\" tö äççéss thïs téäm ässïgnmént.\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяι#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_open.html
+#: templates/openassessmentblock/message/oa_message_open.html
 #, python-format
 msgid ""
 "\n"
 "                    Assignment submissions will close soon. To receive a grade, first provide a response to the prompt, then complete the steps below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 "\n"
 "                    Àssïgnmént süßmïssïöns wïll çlösé söön. Tö réçéïvé ä grädé, fïrst prövïdé ä réspönsé tö thé prömpt, thén çömplété thé stéps ßélöw thé %(start_tag)sÝöür Réspönsé%(end_tag)s fïéld.\n"
 "                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_open.html
+#: templates/openassessmentblock/message/oa_message_open.html
 #, python-format
 msgid ""
 "\n"
 "                    This assignment has several steps. In the first step, you'll provide a response to the prompt. The other steps appear below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 "\n"
 "                    Thïs ässïgnmént häs sévéräl stéps. Ìn thé fïrst stép, ýöü'll prövïdé ä réspönsé tö thé prömpt. Thé öthér stéps äppéär ßélöw thé %(start_tag)sÝöür Réspönsé%(end_tag)s fïéld.\n"
 "                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ησ#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+#: templates/openassessmentblock/message/oa_message_unavailable.html
 msgid "Instructions Unavailable"
 msgstr "Ìnstrüçtïöns Ûnäväïläßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+#: templates/openassessmentblock/message/oa_message_unavailable.html
 msgid "The instructions for this step could not be loaded."
 msgstr ""
 "Thé ïnstrüçtïöns för thïs stép çöüld nöt ßé löädéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/oa_base.html
+#: templates/openassessmentblock/oa_base.html
 msgid ""
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 "Thïs ässïgnmént häs sévéräl stéps. Ìn thé fïrst stép, ýöü'll prövïdé ä "
 "réspönsé tö thé prömpt. Thé öthér stéps äppéär ßélöw thé Ýöür Réspönsé "
 "fïéld. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ "
 "єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм"
 " νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα "
 "¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт"
 " єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт "
 "¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм#"
 
-#: openassessment/templates/openassessmentblock/oa_base.html
+#: templates/openassessmentblock/oa_base.html
 msgid "Loading"
 msgstr "Löädïng Ⱡ'σяєм ιρѕυм #"
 
-#: openassessment/templates/openassessmentblock/oa_latex_preview.html
+#: templates/openassessmentblock/oa_latex_preview.html
 msgid "Preview in LaTeX"
 msgstr "Prévïéw ïn LäTéX Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/oa_latex_preview.html
+#: templates/openassessmentblock/oa_latex_preview.html
 msgid "Click to preview your submission in LaTeX."
 msgstr ""
 "Çlïçk tö prévïéw ýöür süßmïssïön ïn LäTéX. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/oa_latex_preview.html
+#: templates/openassessmentblock/oa_latex_preview.html
 msgid "Preview Response"
 msgstr "Prévïéw Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/oa_rubric.html
+#: templates/openassessmentblock/oa_rubric.html
 msgid "Comments"
 msgstr "Çömménts Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/oa_submission_answer.html
+#: templates/openassessmentblock/oa_submission_answer.html
 msgid "The question for this section"
 msgstr "Thé qüéstïön för thïs séçtïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+#: templates/openassessmentblock/oa_team_uploaded_files.html
 msgid "Files that were uploaded by your teammates:"
 msgstr ""
 "Fïlés thät wéré üplöädéd ßý ýöür téämmätés: Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
-#: openassessment/templates/openassessmentblock/oa_uploaded_file.html
+#: templates/openassessmentblock/oa_team_uploaded_files.html
+#: templates/openassessmentblock/oa_uploaded_file.html
 msgid "View the files associated with this submission:"
 msgstr ""
 "Vïéw thé fïlés ässöçïätéd wïth thïs süßmïssïön: Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
 " ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+#: templates/openassessmentblock/oa_team_uploaded_files.html
 msgid "Uploaded by"
 msgstr "Ûplöädéd ßý Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/oa_uploaded_file.html
+#: templates/openassessmentblock/oa_uploaded_file.html
 msgid "Files that were uploaded by you:"
 msgstr ""
 "Fïlés thät wéré üplöädéd ßý ýöü: Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/oa_uploaded_file.html
+#: templates/openassessmentblock/oa_uploaded_file.html
 msgid ""
 "Caution: These files were uploaded by another course learner and have not "
 "been verified, screened, approved, reviewed, or endorsed by the site "
 "administrator. If you access the files, you do so at your own risk.)"
 msgstr ""
 "Çäütïön: Thésé fïlés wéré üplöädéd ßý änöthér çöürsé léärnér änd hävé nöt "
 "ßéén vérïfïéd, sçréénéd, äpprövéd, révïéwéd, ör éndörséd ßý thé sïté "
 "ädmïnïsträtör. Ìf ýöü äççéss thé fïlés, ýöü dö sö ät ýöür öwn rïsk.) Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρт#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
 msgid "Assess Peers"
 msgstr "Àsséss Péérs Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 00:00 UTC (in
 #. 5 days and 45 minutes)"
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "due August 13th, 2014 00:00 UTC (in 5 days
 #. and 45 minutes)"
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline_peer\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
 #, python-format
 msgid ""
 "\n"
 "                    In Progress (%(review_number)s of %(num_must_grade)s)\n"
 "                "
 msgstr ""
 "\n"
 "                    Ìn Prögréss (%(review_number)s öf %(num_must_grade)s)\n"
 "                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
 msgid "Read and assess the following response from one of your peers."
 msgstr ""
 "Réäd änd ässéss thé föllöwïng réspönsé fröm öné öf ýöür péérs. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Associated Files"
 msgstr "Àssöçïätéd Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_assessment.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "We could not submit your assessment"
 msgstr ""
 "Wé çöüld nöt süßmït ýöür ässéssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
-#: openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
-#: openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
-#: openassessment/xblock/staff_assessment_mixin.py
+#: templates/openassessmentblock/peer/oa_peer_cancelled.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/self/oa_self_cancelled.html
+#: templates/openassessmentblock/student_training/student_training_cancelled.html
+#: xblock/staff_assessment_mixin.py
 msgid "Cancelled"
 msgstr "Çänçélléd Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+#: templates/openassessmentblock/peer/oa_peer_closed.html
 #, python-format
 msgid ""
 "\n"
 "            Incomplete (%(num_graded)s of %(num_must_grade)s)\n"
 "        "
 msgstr ""
 "\n"
 "            Ìnçömplété (%(num_graded)s öf %(num_must_grade)s)\n"
 "         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+#: templates/openassessmentblock/peer/oa_peer_closed.html
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 "Thé düé däté för thïs stép häs pässéd. Thïs stép ïs nöw çlöséd. Ýöü çän nö "
 "löngér çömplété péér ässéssménts ör çöntïnüé wïth thïs ässïgnmént, änd ýöü "
 "wïll réçéïvé ä grädé öf Ìnçömplété. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя"
 " α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє "
 "мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ "
 "łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη "
 "яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα "
 "ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+#: templates/openassessmentblock/peer/oa_peer_complete.html
 msgid "Completed"
 msgstr "Çömplétéd Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_complete.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
 "Completing additional assessments will not affect your final grade."
 msgstr ""
 "Ýöü hävé süççéssfüllý çömplétéd äll öf thé réqüïréd péér ässéssménts för "
 "thïs ässïgnmént. Ýöü mäý ässéss äddïtïönäl péér réspönsés ïf ýöü wänt tö. "
 "Çömplétïng äddïtïönäl ässéssménts wïll nöt äfféçt ýöür fïnäl grädé. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. є#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+#: templates/openassessmentblock/peer/oa_peer_complete.html
 msgid "We could not retrieve additional submissions for assessment"
 msgstr ""
 "Wé çöüld nöt rétrïévé äddïtïönäl süßmïssïöns för ässéssmént Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+#: templates/openassessmentblock/peer/oa_peer_complete.html
 msgid "Continue Assessing Peers"
 msgstr "Çöntïnüé Àsséssïng Péérs Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
 #, python-format
 msgid ""
 "\n"
 "        Complete (%(num_graded)s)\n"
 "      "
 msgstr ""
 "\n"
 "        Çömplété (%(num_graded)s)\n"
 "       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
 msgid ""
 "All submitted peer responses have been assessed. Check back later to see if "
 "more learners have submitted responses."
 msgstr ""
 "Àll süßmïttéd péér réspönsés hävé ßéén ässésséd. Çhéçk ßäçk lätér tö séé ïf "
 "möré léärnérs hävé süßmïttéd réspönsés. Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
-#: openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
-#: openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
-#: openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
-#: openassessment/xblock/staff_assessment_mixin.py
-#: openassessment/xblock/staff_assessment_mixin.py
+#: templates/openassessmentblock/peer/oa_peer_unavailable.html
+#: templates/openassessmentblock/response/oa_response_unavailable.html
+#: templates/openassessmentblock/self/oa_self_unavailable.html
+#: templates/openassessmentblock/student_training/student_training_unavailable.html
+#: xblock/staff_assessment_mixin.py xblock/staff_assessment_mixin.py
 msgid "Not Available"
 msgstr "Nöt Àväïläßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_waiting.html
 #, python-format
 msgid ""
 "\n"
 "          In Progress (%(review_number)s of %(num_must_grade)s)\n"
 "        "
 msgstr ""
 "\n"
 "          Ìn Prögréss (%(review_number)s öf %(num_must_grade)s)\n"
 "         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+#: templates/openassessmentblock/peer/oa_peer_waiting.html
 msgid ""
 "All available peer responses have been assessed. Check back later to see if "
 "more learners have submitted responses. You will receive your grade after "
 "you've completed all the steps for this problem and your peers have assessed"
 " your response."
 msgstr ""
 "Àll äväïläßlé péér réspönsés hävé ßéén ässésséd. Çhéçk ßäçk lätér tö séé ïf "
@@ -1612,164 +1611,165 @@
 "ýöü'vé çömplétéd äll thé stéps för thïs prößlém änd ýöür péérs hävé ässésséd"
 " ýöür réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, "
 "ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм "
 "α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ "
 "єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє"
 " νєłιт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Your Team's Response"
 msgstr "Ýöür Téäm's Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
 #. minutes)"
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 msgid "In Progress"
 msgstr "Ìn Prögréss Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Enter your team's response to the prompt."
 msgstr ""
 "Éntér ýöür téäm's réspönsé tö thé prömpt. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
-"                        You can save your progress and return to complete your team's response at any time before the due date\n"
+"                        Your work will save automatically and you can return to complete your team's response at any time before the due date\n"
 "                      "
 msgstr ""
 "\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété ýöür téäm's réspönsé ät äný tïmé ßéföré thé düé däté\n"
-"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αη#"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn tö çömplété ýöür téäm's réspönsé ät äný tïmé ßéföré thé düé däté\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
-"                        You can save your progress and return to complete your team's response at any time.\n"
+"                        Your work will save automatically and you can return to complete your team's response at any time.\n"
 "                      "
 msgstr ""
 "\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété ýöür téäm's réspönsé ät äný tïmé.\n"
-"                       Ⱡ#"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn tö çömplété ýöür téäm's réspönsé ät äný tïmé.\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
-"After you submit a response on behalf of your team, it cannot be edited"
+"After you submit a response on behalf of your team, it cannot be edited."
 msgstr ""
-"Àftér ýöü süßmït ä réspönsé ön ßéhälf öf ýöür téäm, ït çännöt ßé édïtéd "
+"Àftér ýöü süßmït ä réspönsé ön ßéhälf öf ýöür téäm, ït çännöt ßé édïtéd. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Enter your response to the prompt."
 msgstr ""
 "Éntér ýöür réspönsé tö thé prömpt. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
-"                        You can save your progress and return to complete your response at any time before the due date\n"
+"                        Your work will save automatically and you can return to complete your response at any time before the due date\n"
 "                      "
 msgstr ""
 "\n"
-"                        Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété ýöür réspönsé ät äný tïmé ßéföré thé düé däté\n"
-"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕ#"
+"                        Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn tö çömplété ýöür réspönsé ät äný tïmé ßéföré thé düé däté\n"
+"                       Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
-"You can save your progress and return to complete your response at any time."
+"Your work will save automatically and you can return to complete your "
+"response at any time."
 msgstr ""
-"Ýöü çän sävé ýöür prögréss änd rétürn tö çömplété ýöür réspönsé ät äný tïmé."
-" Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
+"Ýöür wörk wïll sävé äütömätïçällý änd ýöü çän rétürn tö çömplété ýöür "
+"réspönsé ät äný tïmé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "After you submit your response, you cannot edit it"
 msgstr ""
 "Àftér ýöü süßmït ýöür réspönsé, ýöü çännöt édït ït Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "What will this assignment be graded on?"
 msgstr ""
 "Whät wïll thïs ässïgnmént ßé grädéd ön? Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "The prompt for this section"
 msgstr "Thé prömpt för thïs séçtïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "You are on team "
 msgstr "Ýöü äré ön téäm  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Team Members: "
 msgstr "Téäm Mémßérs:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 #, python-format
 msgid ""
 "\n"
 "                                              %(team_members_with_external_submissions)s\n"
 "                                              have/has already submitted a response to this assignment with another team,\n"
 "                                              and will not be a part of your team's submission or assignment grade.\n"
 "                                          "
 msgstr ""
 "\n"
 "                                              %(team_members_with_external_submissions)s\n"
 "                                              hävé/häs älréädý süßmïttéd ä réspönsé tö thïs ässïgnmént wïth änöthér téäm,\n"
 "                                              änd wïll nöt ßé ä pärt öf ýöür téäm's süßmïssïön ör ässïgnmént grädé.\n"
 "                                           Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє є#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Team Response "
 msgstr "Téäm Réspönsé  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Your Response "
 msgstr "Ýöür Réspönsé  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "(Required)"
 msgstr "(Réqüïréd) Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "(Optional)"
 msgstr "(Öptïönäl) Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
 "                                              Teams should designate one team member to submit a response on behalf of the\n"
 "                                              entire team.  All team members can use this space to work on draft responses,\n"
 "                                              but you will not be able to see your teammates' drafts made in this space, so\n"
 "                                              please coordinate with them to decide on the final response the designated team\n"
 "                                              member should submit.\n"
@@ -1779,21 +1779,21 @@
 "                                              Téäms shöüld désïgnäté öné téäm mémßér tö süßmït ä réspönsé ön ßéhälf öf thé\n"
 "                                              éntïré téäm.  Àll téäm mémßérs çän üsé thïs späçé tö wörk ön dräft réspönsés,\n"
 "                                              ßüt ýöü wïll nöt ßé äßlé tö séé ýöür téämmätés' dräfts mädé ïn thïs späçé, sö\n"
 "                                              pléäsé çöördïnäté wïth thém tö déçïdé ön thé fïnäl réspönsé thé désïgnätéd téäm\n"
 "                                              mémßér shöüld süßmït.\n"
 "                                          #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Enter your response to the prompt above."
 msgstr ""
 "Éntér ýöür réspönsé tö thé prömpt äßövé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 #, python-format
 msgid ""
 "\n"
 "                                      You are currently on Team %(team_name)s. Since you were on Team %(previous_team_name)s\n"
 "                                      when they submitted a response to this assignment, you are seeing Team %(previous_team_name)s’s\n"
 "                                      response and will receive the same grade for this assignment as your former teammates.\n"
 "                                      You will not be part of Team %(team_name)s’s submission for this assignment and will not\n"
@@ -1804,258 +1804,247 @@
 "                                      Ýöü äré çürréntlý ön Téäm %(team_name)s. Sïnçé ýöü wéré ön Téäm %(previous_team_name)s\n"
 "                                      whén théý süßmïttéd ä réspönsé tö thïs ässïgnmént, ýöü äré sééïng Téäm %(previous_team_name)s’s\n"
 "                                      réspönsé änd wïll réçéïvé thé sämé grädé för thïs ässïgnmént äs ýöür förmér téämmätés.\n"
 "                                      Ýöü wïll nöt ßé pärt öf Téäm %(team_name)s’s süßmïssïön för thïs ässïgnmént änd wïll nöt\n"
 "                                      réçéïvé ä grädé för théïr süßmïssïön.\n"
 "                                  #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "We could not save your progress"
 msgstr "Wé çöüld nöt sävé ýöür prögréss Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-msgid "Save your progress"
-msgstr "Sävé ýöür prögréss Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
-
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-msgid "Your Submission Status"
-msgstr "Ýöür Süßmïssïön Stätüs Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
+#: templates/openassessmentblock/response/oa_response.html
+msgid "Status of Your Response"
+msgstr "Stätüs öf Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "File Uploads "
 msgstr "Fïlé Ûplöäds  Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
 "                                  Upload files and review files uploaded by you and your teammates below. Be sure to add\n"
 "                                  descriptions to your files to help your teammates identify them.\n"
 "                              "
 msgstr ""
 "\n"
 "                                  Ûplöäd fïlés änd révïéw fïlés üplöädéd ßý ýöü änd ýöür téämmätés ßélöw. Bé süré tö ädd\n"
 "                                  désçrïptïöns tö ýöür fïlés tö hélp ýöür téämmätés ïdéntïfý thém.\n"
 "                               Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "We could not upload files"
 msgstr "Wé çöüld nöt üplöäd fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "We could not delete files"
 msgstr "Wé çöüld nöt délété fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Select one or more files to upload for this submission."
 msgstr ""
 "Séléçt öné ör möré fïlés tö üplöäd för thïs süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Select a file to upload for this submission."
 msgstr ""
 "Séléçt ä fïlé tö üplöäd för thïs süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Supported file types: "
 msgstr "Süppörtéd fïlé týpés:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Upload files"
 msgstr "Ûplöäd fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Upload file"
 msgstr "Ûplöäd fïlé Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
-msgid "You may continue to work on your response until you submit it."
-msgstr ""
-"Ýöü mäý çöntïnüé tö wörk ön ýöür réspönsé üntïl ýöü süßmït ït. Ⱡ'σяєм ιρѕυм "
-"∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
-
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "This is a team submission."
 msgstr "Thïs ïs ä téäm süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "One team member should submit a response with the team’s shared files and a "
 "text response on behalf of the entire team."
 msgstr ""
 "Öné téäm mémßér shöüld süßmït ä réspönsé wïth thé téäm’s shäréd fïlés änd ä "
 "téxt réspönsé ön ßéhälf öf thé éntïré téäm. Ⱡ'σяєм ιρѕυм#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "One team member should submit a response with the team’s shared files on "
 "behalf of the entire team."
 msgstr ""
 "Öné téäm mémßér shöüld süßmït ä réspönsé wïth thé téäm’s shäréd fïlés ön "
 "ßéhälf öf thé éntïré téäm. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "One team member should submit a text response on behalf of the entire team."
 msgstr ""
 "Öné téäm mémßér shöüld süßmït ä téxt réspönsé ön ßéhälf öf thé éntïré téäm. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "One team member should submit on behalf of the entire team."
 msgstr ""
 "Öné téäm mémßér shöüld süßmït ön ßéhälf öf thé éntïré téäm. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid ""
 "\n"
 "                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
 msgstr ""
 "\n"
 "                  Léärn möré äßöüt téäm ässïgnménts héré: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">lïnk</a>)\n"
 "                   Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "We could not submit your response"
 msgstr ""
 "Wé çöüld nöt süßmït ýöür réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response.html
+#: templates/openassessmentblock/response/oa_response.html
 msgid "Submit your response and move to the next step"
 msgstr ""
 "Süßmït ýöür réspönsé änd mövé tö thé néxt stép Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
 msgid "Your submission was cancelled. "
 msgstr "Ýöür süßmïssïön wäs çänçélléd.  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
 #, python-format
 msgid ""
 "\n"
 "                                Your submission has been cancelled by %(removed_by_username)s on %(removed_datetime)s\n"
 "                            "
 msgstr ""
 "\n"
 "                                Ýöür süßmïssïön häs ßéén çänçélléd ßý %(removed_by_username)s ön %(removed_datetime)s\n"
 "                             Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
 #, python-format
 msgid ""
 "\n"
 "                               Your submission was cancelled on %(removed_datetime)s\n"
 "                            "
 msgstr ""
 "\n"
 "                               Ýöür süßmïssïön wäs çänçélléd ön %(removed_datetime)s\n"
 "                             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+#: templates/openassessmentblock/response/oa_response_cancelled.html
 #, python-format
 msgid ""
 "\n"
 "                            Comments: %(comments)s\n"
 "                        "
 msgstr ""
 "\n"
 "                            Çömménts: %(comments)s\n"
 "                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_closed.html
-#: openassessment/templates/openassessmentblock/self/oa_self_closed.html
-#: openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+#: templates/openassessmentblock/response/oa_response_closed.html
+#: templates/openassessmentblock/self/oa_self_closed.html
+#: templates/openassessmentblock/student_training/student_training_closed.html
 msgid "Incomplete"
 msgstr "Ìnçömplété Ⱡ'σяєм ιρѕυм ∂σłσ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_closed.html
+#: templates/openassessmentblock/response/oa_response_closed.html
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
 msgstr ""
 "Thé düé däté för thïs stép häs pässéd. Thïs stép ïs nöw çlöséd. Ýöü çän nö "
 "löngér süßmït ä réspönsé ör çöntïnüé wïth thïs prößlém, änd ýöü wïll réçéïvé"
 " ä grädé öf Ìnçömplété. Ìf ýöü sävéd ßüt dïd nöt süßmït ä réspönsé, thé "
 "réspönsé äppéärs ïn thé çöürsé réçörds. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_graded.html
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
-#: openassessment/templates/openassessmentblock/self/oa_self_complete.html
-#: openassessment/templates/openassessmentblock/student_training/student_training_complete.html
-#: openassessment/xblock/staff_assessment_mixin.py
-#: openassessment/xblock/staff_assessment_mixin.py
+#: templates/openassessmentblock/response/oa_response_graded.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/self/oa_self_complete.html
+#: templates/openassessmentblock/student_training/student_training_complete.html
+#: xblock/staff_assessment_mixin.py xblock/staff_assessment_mixin.py
 msgid "Complete"
 msgstr "Çömplété Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_graded.html
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/response/oa_response_graded.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 msgid "Your response"
 msgstr "Ýöür réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_graded.html
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_graded.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
 msgid "Your Uploaded Files"
 msgstr "Ýöür Ûplöädéd Fïlés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
 msgid ""
 "Your response has been submitted. You will receive your grade after all "
 "steps are complete and your response is fully assessed."
 msgstr ""
 "Ýöür réspönsé häs ßéén süßmïttéd. Ýöü wïll réçéïvé ýöür grädé äftér äll "
 "stéps äré çömplété änd ýöür réspönsé ïs füllý ässésséd. Ⱡ'σяє#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(peer_start_tag)speer assessment%(end_tag)s and %(self_start_tag)sself assessment%(end_tag)s steps.\n"
 "                    "
 msgstr ""
 "\n"
 "                        Ýöü stïll nééd tö çömplété thé %(peer_start_tag)spéér ässéssmént%(end_tag)s änd %(self_start_tag)ssélf ässéssmént%(end_tag)s stéps.\n"
 "                     Ⱡ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(start_tag)speer assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 "\n"
 "                        Ýöü stïll nééd tö çömplété thé %(start_tag)spéér ässéssmént%(end_tag)s stép.\n"
 "                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+#: templates/openassessmentblock/response/oa_response_submitted.html
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(start_tag)sself assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 "\n"
 "                        Ýöü stïll nééd tö çömplété thé %(start_tag)ssélf ässéssmént%(end_tag)s stép.\n"
 "                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+#: templates/openassessmentblock/response/oa_response_team_already_submitted.html
 msgid "Error"
 msgstr "Érrör Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+#: templates/openassessmentblock/response/oa_response_team_already_submitted.html
 #, python-format
 msgid ""
 "\n"
 "                            You joined Team %(team_name)s after they submitted a response for this assignment\n"
 "                            and you will not receive a grade for their response. You have also not previously submitted\n"
 "                            a response to this assignment with another team. Please contact course staff to discuss your\n"
 "                            options for this assignment.\n"
@@ -2064,366 +2053,366 @@
 "\n"
 "                            Ýöü jöïnéd Téäm %(team_name)s äftér théý süßmïttéd ä réspönsé för thïs ässïgnmént\n"
 "                            änd ýöü wïll nöt réçéïvé ä grädé för théïr réspönsé. Ýöü hävé älsö nöt prévïöüslý süßmïttéd\n"
 "                            ä réspönsé tö thïs ässïgnmént wïth änöthér téäm. Pléäsé çöntäçt çöürsé stäff tö dïsçüss ýöür\n"
 "                            öptïöns för thïs ässïgnmént.\n"
 "                        #"
 
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 msgid "Assess Your Response"
 msgstr "Àsséss Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "           "
 msgstr ""
 "\n"
 "               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
 #. minutes)"
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "           "
 msgstr ""
 "\n"
 "               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+#: templates/openassessmentblock/self/oa_self_assessment.html
 msgid "Submit your assessment"
 msgstr "Süßmït ýöür ässéssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/self/oa_self_closed.html
+#: templates/openassessmentblock/self/oa_self_closed.html
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete a self assessment or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 "Thé düé däté för thïs stép häs pässéd. Thïs stép ïs nöw çlöséd. Ýöü çän nö "
 "löngér çömplété ä sélf ässéssmént ör çöntïnüé wïth thïs ässïgnmént, änd ýöü "
 "wïll réçéïvé ä grädé öf Ìnçömplété. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя"
 " α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє "
 "мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ "
 "łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη "
 "яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα "
 "ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂є#"
 
-#: openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
-#: openassessment/xblock/grade_mixin.py
+#: templates/openassessmentblock/staff/oa_staff_grade.html
+#: xblock/grade_mixin.py
 msgid "Staff Grade"
 msgstr "Stäff Grädé Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Manage Individual Learners"
 msgstr "Mänägé Ìndïvïdüäl Léärnérs Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Manage Team Responses"
 msgstr "Mänägé Téäm Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "View Assignment Statistics"
 msgstr "Vïéw Àssïgnmént Stätïstïçs Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Demo the new Grading Experience"
 msgstr "Démö thé néw Grädïng Éxpérïénçé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "View ORA in Studio"
 msgstr "Vïéw ÖRÀ ïn Stüdïö Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Close"
 msgstr "Çlösé Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Manage Teams"
 msgstr "Mänägé Téäms Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Enter an individual learner's username or email"
 msgstr ""
 "Éntér än ïndïvïdüäl léärnér's üsérnämé ör émäïl Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
 " ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Enter a team member's username or edX email"
 msgstr ""
 "Éntér ä téäm mémßér's üsérnämé ör édX émäïl Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Submit"
 msgstr "Süßmït Ⱡ'σяєм ιρѕυ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Response total"
 msgstr "Réspönsé tötäl Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Location"
 msgstr "Löçätïön Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Learner Progress"
 msgstr "Léärnér Prögréss Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Problem Step"
 msgstr "Prößlém Stép Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Active Learners in Step"
 msgstr "Àçtïvé Léärnérs ïn Stép Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Dates"
 msgstr "Dätés Ⱡ'σяєм ιρѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "Release Date"
 msgstr "Réléäsé Däté Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
+#: templates/openassessmentblock/staff_area/oa_staff_area.html
 msgid "N/A"
 msgstr "N/À Ⱡ'σяєм#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
 msgid "Staff Assessment"
 msgstr "Stäff Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
 msgid "Give this team a grade using the problem's rubric."
 msgstr ""
 "Gïvé thïs téäm ä grädé üsïng thé prößlém's rüßrïç. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
 msgid "Give this learner a grade using the problem's rubric."
 msgstr ""
 "Gïvé thïs léärnér ä grädé üsïng thé prößlém's rüßrïç. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт"
 " αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
 #, python-format
 msgid ""
 "\n"
 "                                        Response for: %(team_name)s with %(team_usernames)s\n"
 "                                    "
 msgstr ""
 "\n"
 "                                        Réspönsé för: %(team_name)s wïth %(team_usernames)s\n"
 "                                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 #, python-format
 msgid ""
 "\n"
 "                                        Response for: %(student_username)s\n"
 "                                    "
 msgstr ""
 "\n"
 "                                        Réspönsé för: %(student_username)s\n"
 "                                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "Learner Response"
 msgstr "Léärnér Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
 msgid "The teams's response to the prompt above"
 msgstr ""
 "Thé téäms's réspönsé tö thé prömpt äßövé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "The learner's response to the prompt above"
 msgstr ""
 "Thé léärnér's réspönsé tö thé prömpt äßövé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "Submit assessment"
 msgstr "Süßmït ässéssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
 msgid "Submit assessment and continue grading"
 msgstr ""
 "Süßmït ässéssmént änd çöntïnüé grädïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
+#: templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
 #, python-format
 msgid ""
 "\n"
 "                %(ungraded)s Available and %(in_progress)s Checked Out\n"
 "            "
 msgstr ""
 "\n"
 "                %(ungraded)s Àväïläßlé änd %(in_progress)s Çhéçkéd Öüt\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "Override this learner's current grade using the problem's rubric."
 msgstr ""
 "Övérrïdé thïs léärnér's çürrént grädé üsïng thé prößlém's rüßrïç. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "Override this team's current grade using the problem's rubric."
 msgstr ""
 "Övérrïdé thïs téäm's çürrént grädé üsïng thé prößlém's rüßrïç. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
 msgid "Team Response"
 msgstr "Téäm Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "The team's response to the prompt above"
 msgstr ""
 "Thé téäm's réspönsé tö thé prömpt äßövé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                    Viewing learner: %(learner)s\n"
 "                "
 msgstr ""
 "\n"
 "                    Vïéwïng léärnér: %(learner)s\n"
 "                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                    Viewing team: %(team)s\n"
 "                "
 msgstr ""
 "\n"
 "                    Vïéwïng téäm: %(team)s\n"
 "                 Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Learner's Response"
 msgstr "Léärnér's Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Team's Response"
 msgstr "Téäm's Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                            Learner submission removed by %(removed_by_username)s on %(removed_datetime)s\n"
 "                        "
 msgstr ""
 "\n"
 "                            Léärnér süßmïssïön rémövéd ßý %(removed_by_username)s ön %(removed_datetime)s\n"
 "                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                            Learner submission removed on %(removed_datetime)s\n"
 "                        "
 msgstr ""
 "\n"
 "                            Léärnér süßmïssïön rémövéd ön %(removed_datetime)s\n"
 "                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                        Comments: %(comments)s\n"
 "                    "
 msgstr ""
 "\n"
 "                        Çömménts: %(comments)s\n"
 "                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Peer Assessments for This Learner"
 msgstr ""
 "Péér Àsséssménts för Thïs Léärnér Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Peer Assessments Completed by This Learner"
 msgstr ""
 "Péér Àsséssménts Çömplétéd ßý Thïs Léärnér Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Learner's Self Assessment"
 msgstr "Léärnér's Sélf Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Staff Assessment for This Learner"
 msgstr ""
 "Stäff Àsséssmént för Thïs Léärnér Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Staff Assessment for this Team"
 msgstr "Stäff Àsséssmént för thïs Téäm Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Learner's Final Grade"
 msgstr "Léärnér's Fïnäl Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Team's Final Grade"
 msgstr "Téäm's Fïnäl Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                            Final grade: %(points_earned)s out of %(points_possible)s\n"
 "                        "
 msgstr ""
 "\n"
 "                            Fïnäl grädé: %(points_earned)s öüt öf %(points_possible)s\n"
 "                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Final Grade Details"
 msgstr "Fïnäl Grädé Détäïls Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 #, python-format
 msgid ""
 "\n"
 "                                        %(assessment_label)s - %(points)s point\n"
 "                                    "
 msgid_plural ""
 "\n"
@@ -2434,1050 +2423,1038 @@
 "                                        %(assessment_label)s - %(points)s pöïnt\n"
 "                                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 msgstr[1] ""
 "\n"
 "                                        %(assessment_label)s - %(points)s pöïnts\n"
 "                                     Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Feedback Recorded"
 msgstr "Féédßäçk Réçördéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "The submission is waiting for assessments."
 msgstr ""
 "Thé süßmïssïön ïs wäïtïng för ässéssménts. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "The learner's submission has been removed from peer assessment. The learner "
 "receives a grade of zero unless you delete the learner's state for the "
 "problem to allow them to resubmit a response."
 msgstr ""
 "Thé léärnér's süßmïssïön häs ßéén rémövéd fröm péér ässéssmént. Thé léärnér "
 "réçéïvés ä grädé öf zérö ünléss ýöü délété thé léärnér's stäté för thé "
 "prößlém tö ällöw thém tö résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
 " ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ησ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "The team’s submission has been removed from grading. The team receives a "
 "grade of zero unless you delete the a team member’s state for the problem to"
 " allow the team to resubmit a response."
 msgstr ""
 "Thé téäm’s süßmïssïön häs ßéén rémövéd fröm grädïng. Thé téäm réçéïvés ä "
 "grädé öf zérö ünléss ýöü délété thé ä téäm mémßér’s stäté för thé prößlém tö"
 " ällöw thé téäm tö résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
 " ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "The problem has not been started."
 msgstr ""
 "Thé prößlém häs nöt ßéén stärtéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "The problem has not been completed."
 msgstr ""
 "Thé prößlém häs nöt ßéén çömplétéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Submit Assessment Grade Override"
 msgstr ""
 "Süßmït Àsséssmént Grädé Övérrïdé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Submit Team Grade Override"
 msgstr "Süßmït Téäm Grädé Övérrïdé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Unable to perform grade override"
 msgstr ""
 "Ûnäßlé tö pérförm grädé övérrïdé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "Grades are frozen. Grades are automatically frozen 30 days after the course "
 "end date."
 msgstr ""
 "Grädés äré frözén. Grädés äré äütömätïçällý frözén 30 däýs äftér thé çöürsé "
 "énd däté. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "This submission has been cancelled and cannot recieve a grade. Refer to "
 "documentation for how to delete the learner’s state for this problem to "
 "allow them to resubmit."
 msgstr ""
 "Thïs süßmïssïön häs ßéén çänçélléd änd çännöt réçïévé ä grädé. Référ tö "
 "döçüméntätïön för höw tö délété thé léärnér’s stäté för thïs prößlém tö "
 "ällöw thém tö résüßmït. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg"
 " єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт"
 " єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт "
 "αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη "
 "νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт "
 "σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Remove Submission From Peer Grading"
 msgstr ""
 "Rémövé Süßmïssïön Fröm Péér Grädïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Remove Team Submission from Grading"
 msgstr ""
 "Rémövé Téäm Süßmïssïön fröm Grädïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Caution: This Action Cannot Be Undone"
 msgstr ""
 "Çäütïön: Thïs Àçtïön Çännöt Bé Ûndöné Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "Removing a learner's submission cannot be undone and should be done with "
 "caution."
 msgstr ""
 "Rémövïng ä léärnér's süßmïssïön çännöt ßé ündöné änd shöüld ßé döné wïth "
 "çäütïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid ""
 "Removing a team's submission cannot be undone and should be done with "
 "caution."
 msgstr ""
 "Rémövïng ä téäm's süßmïssïön çännöt ßé ündöné änd shöüld ßé döné wïth "
 "çäütïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Comments:"
 msgstr "Çömménts: Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "Remove submission"
 msgstr "Rémövé süßmïssïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+#: templates/openassessmentblock/staff_area/oa_student_info.html
 msgid "A response was not found for this learner."
 msgstr ""
 "À réspönsé wäs nöt föünd för thïs léärnér. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 #, python-format
 msgid ""
 "\n"
 "                            Assessment %(assessment_num)s:\n"
 "                        "
 msgstr ""
 "\n"
 "                            Àsséssmént %(assessment_num)s:\n"
 "                         Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Assessment Details"
 msgstr "Àsséssmént Détäïls Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Selected Option"
 msgstr "Séléçtéd Öptïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Feedback"
 msgstr "Féédßäçk Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+#: templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
 msgid "Points Possible"
 msgstr "Pöïnts Pössïßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "Learn to Assess Responses"
 msgstr "Léärn tö Àsséss Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 #, python-format
 msgid ""
 "\n"
 "                      In Progress (%(current_progress_num)s of %(training_available_num)s)\n"
 "                  "
 msgstr ""
 "\n"
 "                      Ìn Prögréss (%(current_progress_num)s öf %(training_available_num)s)\n"
 "                   Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(start_date)s\" data-string=\"available {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "due August 13th, 2014 (in 5 days and 45
 #. minutes)"
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 #, python-format, python-brace-format
 msgid ""
 "\n"
 "            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 "\n"
 "            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "             Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "Learning to Assess Responses"
 msgstr "Léärnïng tö Àsséss Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid ""
 "Before you begin to assess your peers' responses, you'll learn how to "
 "complete peer assessments by reviewing responses that instructors have "
 "already assessed. If you select the same options for the response that the "
 "instructor selected, you'll move to the next step. If you don't select the "
 "same options, you'll review the response and try again."
 msgstr ""
 "Béföré ýöü ßégïn tö ässéss ýöür péérs' réspönsés, ýöü'll léärn höw tö "
 "çömplété péér ässéssménts ßý révïéwïng réspönsés thät ïnstrüçtörs hävé "
 "älréädý ässésséd. Ìf ýöü séléçt thé sämé öptïöns för thé réspönsé thät thé "
 "ïnstrüçtör séléçtéd, ýöü'll mövé tö thé néxt stép. Ìf ýöü dön't séléçt thé "
 "sämé öptïöns, ýöü'll révïéw thé réspönsé änd trý ägäïn. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єι#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid ""
 "Your assessment differs from the instructor's assessment of this response. "
 "Review the response and consider why the instructor may have assessed it "
 "differently. Then, try the assessment again."
 msgstr ""
 "Ýöür ässéssmént dïfférs fröm thé ïnstrüçtör's ässéssmént öf thïs réspönsé. "
 "Révïéw thé réspönsé änd çönsïdér whý thé ïnstrüçtör mäý hävé ässésséd ït "
 "dïfféréntlý. Thén, trý thé ässéssmént ägäïn. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
 " ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ησ#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "The response to the prompt above:"
 msgstr ""
 "Thé réspönsé tö thé prömpt äßövé: Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "Selected Options Agree"
 msgstr "Séléçtéd Öptïöns Àgréé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "The option you selected is the option that the instructor selected."
 msgstr ""
 "Thé öptïön ýöü séléçtéd ïs thé öptïön thät thé ïnstrüçtör séléçtéd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "Selected Options Differ"
 msgstr "Séléçtéd Öptïöns Dïffér Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid ""
 "The option you selected is not the option that the instructor selected."
 msgstr ""
 "Thé öptïön ýöü séléçtéd ïs nöt thé öptïön thät thé ïnstrüçtör séléçtéd. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "We could not check your assessment"
 msgstr ""
 "Wé çöüld nöt çhéçk ýöür ässéssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training.html
+#: templates/openassessmentblock/student_training/student_training.html
 msgid "Compare your selections with the instructor's selections"
 msgstr ""
 "Çömpäré ýöür séléçtïöns wïth thé ïnstrüçtör's séléçtïöns Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+#: templates/openassessmentblock/student_training/student_training_closed.html
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer continue with this assignment, and you will receive a grade of "
 "Incomplete."
 msgstr ""
 "Thé düé däté för thïs stép häs pässéd. Thïs stép ïs nöw çlöséd. Ýöü çän nö "
 "löngér çöntïnüé wïth thïs ässïgnmént, änd ýöü wïll réçéïvé ä grädé öf "
 "Ìnçömplété. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ "
 "∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ "
 "мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ "
 "єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє "
 "νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт "
 "¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσ#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training_error.html
+#: templates/openassessmentblock/student_training/student_training_error.html
 msgid "Error Loading Learner Training Examples"
 msgstr ""
 "Érrör Löädïng Léärnér Träïnïng Éxämplés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/templates/openassessmentblock/student_training/student_training_error.html
+#: templates/openassessmentblock/student_training/student_training_error.html
 msgid "The Learner Training Step of this assignment could not be loaded."
 msgstr ""
 "Thé Léärnér Träïnïng Stép öf thïs ässïgnmént çöüld nöt ßé löädéd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/data_conversion.py
+#: xblock/data_conversion.py
 msgid "You must provide options selected in the assessment."
 msgstr ""
 "Ýöü müst prövïdé öptïöns séléçtéd ïn thé ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/data_conversion.py
+#: xblock/data_conversion.py
 msgid "You must provide overall feedback in the assessment."
 msgstr ""
 "Ýöü müst prövïdé övéräll féédßäçk ïn thé ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/data_conversion.py
+#: xblock/data_conversion.py
 msgid "You must provide feedback for criteria in the assessment."
 msgstr ""
 "Ýöü müst prövïdé féédßäçk för çrïtérïä ïn thé ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя"
 " ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/grade_mixin.py
-#: openassessment/xblock/leaderboard_mixin.py
-#: openassessment/xblock/self_assessment_mixin.py
-#: openassessment/xblock/student_training_mixin.py
-#: openassessment/xblock/student_training_mixin.py
+#: xblock/grade_mixin.py xblock/leaderboard_mixin.py
+#: xblock/self_assessment_mixin.py xblock/student_training_mixin.py
+#: xblock/student_training_mixin.py
 msgid "An unexpected error occurred."
 msgstr "Àn ünéxpéçtéd érrör öççürréd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Peer Assessment"
 msgstr "Péér Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Self Assessment"
 msgstr "Sélf Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Assessment feedback could not be saved."
 msgstr ""
 "Àsséssmént féédßäçk çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Feedback saved."
 msgstr "Féédßäçk sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
 
-#: openassessment/xblock/grade_mixin.py openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py xblock/grade_mixin.py
 msgid "Staff Comments"
 msgstr "Stäff Çömménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Peer Median Grade"
 msgstr "Péér Médïän Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/xblock/grade_mixin.py openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py xblock/grade_mixin.py
 #, python-brace-format
 msgid "Peer {peer_index}"
 msgstr "Péér {peer_index} Ⱡ'σяєм ιρѕυм ∂#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Peer Comments"
 msgstr "Péér Çömménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Self Assessment Grade"
 msgstr "Sélf Àsséssmént Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Your Self Assessment"
 msgstr "Ýöür Sélf Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/grade_mixin.py openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py xblock/grade_mixin.py
 msgid "Your Comments"
 msgstr "Ýöür Çömménts Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Waiting for peer reviews"
 msgstr "Wäïtïng för péér révïéws Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "Peer"
 msgstr "Péér Ⱡ'σяєм ι#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "The grade for this problem is determined by your Staff Grade."
 msgstr ""
 "Thé grädé för thïs prößlém ïs détérmïnéd ßý ýöür Stäff Grädé. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid ""
 "The grade for this problem is determined by the median score of your Peer "
 "Assessments."
 msgstr ""
 "Thé grädé för thïs prößlém ïs détérmïnéd ßý thé médïän sçöré öf ýöür Péér "
 "Àsséssménts. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid "The grade for this problem is determined by your Self Assessment."
 msgstr ""
 "Thé grädé för thïs prößlém ïs détérmïnéd ßý ýöür Sélf Àsséssmént. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 #, python-brace-format
 msgid ""
 "You have successfully completed this problem and received a "
 "{earned_points}/{total_points}."
 msgstr ""
 "Ýöü hävé süççéssfüllý çömplétéd thïs prößlém änd réçéïvéd ä "
 "{earned_points}/{total_points}. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/grade_mixin.py
+#: xblock/grade_mixin.py
 msgid ""
 "You have not yet received all necessary peer reviews to determine your final"
 " grade."
 msgstr ""
 "Ýöü hävé nöt ýét réçéïvéd äll néçéssärý péér révïéws tö détérmïné ýöür fïnäl"
 " grädé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/xblock/openassesment_template_mixin.py
+#: xblock/openassesment_template_mixin.py
 msgid "Peer Assessment Only"
 msgstr "Péér Àsséssmént Önlý Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/openassesment_template_mixin.py
+#: xblock/openassesment_template_mixin.py
 msgid "Self Assessment Only"
 msgstr "Sélf Àsséssmént Önlý Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/openassesment_template_mixin.py
+#: xblock/openassesment_template_mixin.py
 msgid "Staff Assessment Only"
 msgstr "Stäff Àsséssmént Önlý Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/openassesment_template_mixin.py
+#: xblock/openassesment_template_mixin.py
 msgid "Self Assessment to Peer Assessment"
 msgstr ""
 "Sélf Àsséssmént tö Péér Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/openassesment_template_mixin.py
+#: xblock/openassesment_template_mixin.py
 msgid "Self Assessment to Staff Assessment"
 msgstr ""
 "Sélf Àsséssmént tö Stäff Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 msgid "You must submit a response before you can perform a peer assessment."
 msgstr ""
 "Ýöü müst süßmït ä réspönsé ßéföré ýöü çän pérförm ä péér ässéssmént. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 msgid ""
 "This feedback has already been submitted or the submission has been "
 "cancelled."
 msgstr ""
 "Thïs féédßäçk häs älréädý ßéén süßmïttéd ör thé süßmïssïön häs ßéén "
 "çänçélléd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/peer_assessment_mixin.py
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py xblock/peer_assessment_mixin.py
 msgid "Your peer assessment could not be submitted."
 msgstr ""
 "Ýöür péér ässéssmént çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/peer_assessment_mixin.py
-#: openassessment/xblock/student_training_mixin.py
+#: xblock/peer_assessment_mixin.py xblock/student_training_mixin.py
 msgid "Could not update workflow status."
 msgstr ""
 "Çöüld nöt üpdäté wörkflöw stätüs. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 msgid "Could not load peer assessment."
 msgstr "Çöüld nöt löäd péér ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 msgid "Submit your assessment and review another response"
 msgstr ""
 "Süßmït ýöür ässéssmént änd révïéw änöthér réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 msgid "Submit your assessment and move to next step"
 msgstr ""
 "Süßmït ýöür ässéssmént änd mövé tö néxt stép Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/peer_assessment_mixin.py
+#: xblock/peer_assessment_mixin.py
 #, python-brace-format
 msgid "Submit your assessment and move to response #{response_number}"
 msgstr ""
 "Süßmït ýöür ässéssmént änd mövé tö réspönsé #{response_number} Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/resolve_dates.py
+#: xblock/resolve_dates.py
 #, python-brace-format
 msgid ""
 "'{date}' is an invalid date format. Make sure the date is formatted as YYYY-"
 "MM-DDTHH:MM:SS."
 msgstr ""
 "'{date}' ïs än ïnvälïd däté förmät. Mäké süré thé däté ïs förmättéd äs ÝÝÝÝ-"
 "MM-DDTHH:MM:SS. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє#"
 
-#: openassessment/xblock/resolve_dates.py
+#: xblock/resolve_dates.py
 #, python-brace-format
 msgid "'{date}' must be a date string or datetime"
 msgstr ""
 "'{date}' müst ßé ä däté strïng ör dätétïmé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/resolve_dates.py
+#: xblock/resolve_dates.py
 #, python-brace-format
 msgid ""
 "This step's start date '{start}' cannot be earlier than the previous step's "
 "start date '{prev}'."
 msgstr ""
 "Thïs stép's stärt däté '{start}' çännöt ßé éärlïér thän thé prévïöüs stép's "
 "stärt däté '{prev}'. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/xblock/resolve_dates.py
+#: xblock/resolve_dates.py
 #, python-brace-format
 msgid ""
 "This step's due date '{due}' cannot be later than the next step's due date "
 "'{prev}'."
 msgstr ""
 "Thïs stép's düé däté '{due}' çännöt ßé lätér thän thé néxt stép's düé däté "
 "'{prev}'. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/resolve_dates.py
+#: xblock/resolve_dates.py
 #, python-brace-format
 msgid "The start date '{start}' cannot be later than the due date '{due}'"
 msgstr ""
 "Thé stärt däté '{start}' çännöt ßé lätér thän thé düé däté '{due}' Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/rubric_reuse_mixin.py
+#: xblock/rubric_reuse_mixin.py
 msgid "You must specify a block id from which to copy a rubric."
 msgstr ""
 "Ýöü müst spéçïfý ä ßlöçk ïd fröm whïçh tö çöpý ä rüßrïç. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/rubric_reuse_mixin.py
+#: xblock/rubric_reuse_mixin.py
 msgid "Invalid block id."
 msgstr "Ìnvälïd ßlöçk ïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
-#: openassessment/xblock/rubric_reuse_mixin.py
+#: xblock/rubric_reuse_mixin.py
 #, python-brace-format
 msgid ""
 "No Open Response Assessment found in {course_id} with block id {block_id}"
 msgstr ""
 "Nö Öpén Réspönsé Àsséssmént föünd ïn {course_id} wïth ßlöçk ïd {block_id} "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/self_assessment_mixin.py
+#: xblock/self_assessment_mixin.py
 msgid "You must submit a response before you can perform a self-assessment."
 msgstr ""
 "Ýöü müst süßmït ä réspönsé ßéföré ýöü çän pérförm ä sélf-ässéssmént. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/self_assessment_mixin.py
-#: openassessment/xblock/self_assessment_mixin.py
+#: xblock/self_assessment_mixin.py xblock/self_assessment_mixin.py
 msgid "Your self assessment could not be submitted."
 msgstr ""
 "Ýöür sélf ässéssmént çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "You do not have permission to schedule training"
 msgstr ""
 "Ýöü dö nöt hävé pérmïssïön tö sçhédülé träïnïng Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
 " ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "You do not have permission to reschedule tasks."
 msgstr ""
 "Ýöü dö nöt hävé pérmïssïön tö résçhédülé täsks. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
 " ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "You do not have permission to access the ORA staff area"
 msgstr ""
 "Ýöü dö nöt hävé pérmïssïön tö äççéss thé ÖRÀ stäff äréä Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "You do not have permission to access ORA learner information."
 msgstr ""
 "Ýöü dö nöt hävé pérmïssïön tö äççéss ÖRÀ léärnér ïnförmätïön. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "You do not have permission to access ORA staff grading."
 msgstr ""
 "Ýöü dö nöt hävé pérmïssïön tö äççéss ÖRÀ stäff grädïng. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Pending"
 msgstr "Péndïng Ⱡ'σяєм ιρѕυм #"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Complete/Overwritten"
 msgstr "Çömplété/Övérwrïttén Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Not applicable"
 msgstr "Nöt äpplïçäßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Not submitted"
 msgstr "Nöt süßmïttéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Submitted"
 msgstr "Süßmïttéd Ⱡ'σяєм ιρѕυм ∂σł#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Error getting learner information."
 msgstr ""
 "Érrör géttïng léärnér ïnförmätïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Error loading the checked out learner response."
 msgstr ""
 "Érrör löädïng thé çhéçkéd öüt léärnér réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
 " ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "No other learner responses are available for grading at this time."
 msgstr ""
 "Nö öthér léärnér réspönsés äré äväïläßlé för grädïng ät thïs tïmé. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Error getting staff grade information."
 msgstr ""
 "Érrör géttïng stäff grädé ïnförmätïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Error getting staff grade ungraded and checked out counts."
 msgstr ""
 "Érrör géttïng stäff grädé üngrädéd änd çhéçkéd öüt çöünts. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Please enter valid reason to remove the submission."
 msgstr ""
 "Pléäsé éntér välïd réäsön tö rémövé thé süßmïssïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Submission not found"
 msgstr "Süßmïssïön nöt föünd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid "Submission for team assignment has no associated team submission"
 msgstr ""
 "Süßmïssïön för téäm ässïgnmént häs nö ässöçïätéd téäm süßmïssïön Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid ""
 "The learner submission has been removed from peer assessment. The learner "
 "receives a grade of zero unless you delete the learner's state for the "
 "problem to allow them to resubmit a response."
 msgstr ""
 "Thé léärnér süßmïssïön häs ßéén rémövéd fröm péér ässéssmént. Thé léärnér "
 "réçéïvés ä grädé öf zérö ünléss ýöü délété thé léärnér's stäté för thé "
 "prößlém tö ällöw thém tö résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
 " ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρ#"
 
-#: openassessment/xblock/staff_area_mixin.py
+#: xblock/staff_area_mixin.py
 msgid ""
 "The team’s submission has been removed from grading. The team receives a "
 "grade of zero unless you delete a team member’s state for the problem to "
 "allow the team to resubmit a response."
 msgstr ""
 "Thé téäm’s süßmïssïön häs ßéén rémövéd fröm grädïng. Thé téäm réçéïvés ä "
 "grädé öf zérö ünléss ýöü délété ä téäm mémßér’s stäté för thé prößlém tö "
 "ällöw thé téäm tö résüßmït ä réspönsé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
 "∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
 "υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
 "∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
 " ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂єηт,#"
 
-#: openassessment/xblock/staff_assessment_mixin.py
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py xblock/staff_assessment_mixin.py
 msgid "The submission ID of the submission being assessed was not found."
 msgstr ""
 "Thé süßmïssïön ÌD öf thé süßmïssïön ßéïng ässésséd wäs nöt föünd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_assessment_mixin.py
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py xblock/staff_assessment_mixin.py
 msgid "Your staff assessment could not be submitted."
 msgstr ""
 "Ýöür stäff ässéssmént çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/staff_assessment_mixin.py
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py xblock/staff_assessment_mixin.py
 msgid "Your team assessment could not be submitted."
 msgstr ""
 "Ýöür téäm ässéssmént çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py
 msgid "Waiting for a Staff Grade"
 msgstr "Wäïtïng för ä Stäff Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
 
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py
 msgid ""
 "Check back later to see if a course staff member has assessed your response."
 " You will receive your grade after the assessment is complete."
 msgstr ""
 "Çhéçk ßäçk lätér tö séé ïf ä çöürsé stäff mémßér häs ässésséd ýöür réspönsé."
 " Ýöü wïll réçéïvé ýöür grädé äftér thé ässéssmént ïs çömplété. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт łαв#"
 
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py
 msgid "You Must Complete the Steps Above to View Your Grade"
 msgstr ""
 "Ýöü Müst Çömplété thé Stéps Àßövé tö Vïéw Ýöür Grädé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/staff_assessment_mixin.py
+#: xblock/staff_assessment_mixin.py
 msgid ""
 "Although a course staff member has assessed your response, you will receive "
 "your grade only after you have completed all the required steps of this "
 "problem."
 msgstr ""
 "Àlthöügh ä çöürsé stäff mémßér häs ässésséd ýöür réspönsé, ýöü wïll réçéïvé "
 "ýöür grädé önlý äftér ýöü hävé çömplétéd äll thé réqüïréd stéps öf thïs "
 "prößlém. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ "
 "єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм"
 " νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα "
 "¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт"
 " єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт "
 "¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσ#"
 
-#: openassessment/xblock/student_training_mixin.py
+#: xblock/student_training_mixin.py
 msgid "Missing options_selected key in request"
 msgstr ""
 "Mïssïng öptïöns_séléçtéd kéý ïn réqüést Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/student_training_mixin.py
+#: xblock/student_training_mixin.py
 msgid "options_selected must be a dictionary"
 msgstr ""
 "öptïöns_séléçtéd müst ßé ä dïçtïönärý Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/student_training_mixin.py
-#: openassessment/xblock/student_training_mixin.py
+#: xblock/student_training_mixin.py xblock/student_training_mixin.py
 msgid "Your scores could not be checked."
 msgstr ""
 "Ýöür sçörés çöüld nöt ßé çhéçkéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/xblock/studio_mixin.py openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py xblock/studio_mixin.py
 msgid "Error updating XBlock configuration"
 msgstr ""
 "Érrör üpdätïng XBlöçk çönfïgürätïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py
 msgid "Error: Text Response and File Upload Response cannot both be disabled"
 msgstr ""
 "Érrör: Téxt Réspönsé änd Fïlé Ûplöäd Réspönsé çännöt ßöth ßé dïsäßléd Ⱡ'σяєм"
 " ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py
 msgid ""
 "Error: When Text Response is disabled, File Upload Response must be Required"
 msgstr ""
 "Érrör: Whén Téxt Réspönsé ïs dïsäßléd, Fïlé Ûplöäd Réspönsé müst ßé Réqüïréd"
 " Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py
 msgid ""
 "Error: When File Upload Response is disabled, Text Response must be Required"
 msgstr ""
 "Érrör: Whén Fïlé Ûplöäd Réspönsé ïs dïsäßléd, Téxt Réspönsé müst ßé Réqüïréd"
 " Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py
 #, python-brace-format
 msgid "Validation error: {error}"
 msgstr "Välïdätïön érrör: {error} Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/studio_mixin.py
+#: xblock/studio_mixin.py
 msgid "Successfully updated OpenAssessment XBlock"
 msgstr ""
 "Süççéssfüllý üpdätéd ÖpénÀsséssmént XBlöçk Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "\"submission\" required to submit answer."
 msgstr ""
 "\"süßmïssïön\" réqüïréd tö süßmït änswér. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "To submit a response, view this component in Preview or Live mode."
 msgstr ""
 "Tö süßmït ä réspönsé, vïéw thïs çömpönént ïn Prévïéw ör Lïvé mödé. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Multiple submissions are not allowed."
 msgstr ""
 "Mültïplé süßmïssïöns äré nöt ällöwéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Response exceeds maximum allowed size."
 msgstr ""
 "Réspönsé éxçééds mäxïmüm ällöwéd sïzé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid ""
 "Note: if you have a spellcheck or grammar check browser extension, try "
 "disabling, reloading, and reentering your response before submitting."
 msgstr ""
 "Nöté: ïf ýöü hävé ä spéllçhéçk ör grämmär çhéçk ßröwsér éxténsïön, trý "
 "dïsäßlïng, rélöädïng, änd rééntérïng ýöür réspönsé ßéföré süßmïttïng. Ⱡ'σяєм"
 " ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
 "ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
 "ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт ł#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Submission cannot be empty. Please refresh the page and try again."
 msgstr ""
 "Süßmïssïön çännöt ßé émptý. Pléäsé réfrésh thé pägé änd trý ägäïn. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "API returned unclassified exception."
 msgstr ""
 "ÀPÌ rétürnéd ünçlässïfïéd éxçéptïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/submission_mixin.py
-msgid "This response could not be saved."
-msgstr ""
-"Thïs réspönsé çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+#: xblock/submission_mixin.py
+msgid "Please contact support staff."
+msgstr "Pléäsé çöntäçt süppört stäff. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/xblock/submission_mixin.py
-msgid "This response was not submitted."
+#: xblock/submission_mixin.py
+msgid "Submission data missing. Please contact support staff."
 msgstr ""
-"Thïs réspönsé wäs nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+"Süßmïssïön dätä mïssïng. Pléäsé çöntäçt süppört stäff. Ⱡ'σяєм ιρѕυм ∂σłσя "
+"ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Files descriptions were not submitted."
 msgstr ""
 "Fïlés désçrïptïöns wéré nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Files metadata could not be saved."
 msgstr ""
 "Fïlés métädätä çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "There was an error uploading your file."
 msgstr ""
 "Théré wäs än érrör üplöädïng ýöür fïlé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Only a single file upload is allowed for this assessment."
 msgstr ""
 "Önlý ä sïnglé fïlé üplöäd ïs ällöwéd för thïs ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя"
 " ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid ""
 "File upload failed: unsupported file type.Only the supported file types can "
 "be uploaded.If you have questions, please reach out to the course team."
 msgstr ""
 "Fïlé üplöäd fäïléd: ünsüppörtéd fïlé týpé.Önlý thé süppörtéd fïlé týpés çän "
 "ßé üplöädéd.Ìf ýöü hävé qüéstïöns, pléäsé réäçh öüt tö thé çöürsé téäm. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
 "тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
 " qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
 "¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
 "¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
 "ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм #"
 
-#: openassessment/xblock/submission_mixin.py
+#: xblock/submission_mixin.py
 msgid "Error retrieving upload URL."
 msgstr "Érrör rétrïévïng üplöäd ÛRL. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
 
-#: openassessment/xblock/submission_mixin.py
-msgid "This response has been saved but not submitted."
-msgstr ""
-"Thïs réspönsé häs ßéén sävéd ßüt nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
-" ¢σηѕє¢тєтυя α#"
-
-#: openassessment/xblock/submission_mixin.py
-msgid "This response has not been saved."
-msgstr ""
-"Thïs réspönsé häs nöt ßéén sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+#: xblock/submission_mixin.py
+msgid "Draft saved!"
+msgstr "Dräft sävéd! Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+
+#: xblock/submission_mixin.py
+msgid "Response not started."
+msgstr "Réspönsé nöt stärtéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "This problem must include at least one assessment."
 msgstr ""
 "Thïs prößlém müst ïnçlüdé ät léäst öné ässéssmént. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
 "αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "The assessment order you selected is invalid."
 msgstr ""
 "Thé ässéssmént ördér ýöü séléçtéd ïs ïnvälïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "In peer assessment, the \"Must Grade\" value must be a positive integer."
 msgstr ""
 "Ìn péér ässéssmént, thé \"Müst Grädé\" välüé müst ßé ä pösïtïvé ïntégér. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "In peer assessment, the \"Graded By\" value must be a positive integer."
 msgstr ""
 "Ìn péér ässéssmént, thé \"Grädéd Bý\" välüé müst ßé ä pösïtïvé ïntégér. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid ""
 "In peer assessment, the \"Must Grade\" value must be greater than or equal "
 "to the \"Graded By\" value."
 msgstr ""
 "Ìn péér ässéssmént, thé \"Müst Grädé\" välüé müst ßé gréätér thän ör éqüäl "
 "tö thé \"Grädéd Bý\" välüé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "You must provide at least one example response for learner training."
 msgstr ""
 "Ýöü müst prövïdé ät léäst öné éxämplé réspönsé för léärnér träïnïng. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Each example response for learner training must be unique."
 msgstr ""
 "Éäçh éxämplé réspönsé för léärnér träïnïng müst ßé ünïqüé. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "The \"required\" value must be true if staff assessment is the only step."
 msgstr ""
 "Thé \"réqüïréd\" välüé müst ßé trüé ïf stäff ässéssmént ïs thé önlý stép. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid ""
 "The number of assessments cannot be changed after the problem has been "
 "released."
 msgstr ""
 "Thé nümßér öf ässéssménts çännöt ßé çhängéd äftér thé prößlém häs ßéén "
 "réléäséd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid ""
 "The assessment type cannot be changed after the problem has been released."
 msgstr ""
 "Thé ässéssmént týpé çännöt ßé çhängéd äftér thé prößlém häs ßéén réléäséd. "
 "Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "This rubric definition is not valid."
 msgstr ""
 "Thïs rüßrïç défïnïtïön ïs nöt välïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυ#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 #, python-brace-format
 msgid "Options in '{criterion}' have duplicate name(s): {duplicates}"
 msgstr ""
 "Öptïöns ïn '{criterion}' hävé düplïçäté nämé(s): {duplicates} Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Criteria with no options must require written feedback."
 msgstr ""
 "Çrïtérïä wïth nö öptïöns müst réqüïré wrïttén féédßäçk. Ⱡ'σяєм ιρѕυм ∂σłσя "
 "ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Prompts cannot be created or deleted after a problem is released."
 msgstr ""
 "Prömpts çännöt ßé çréätéd ör délétéd äftér ä prößlém ïs réléäséd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "The number of criteria cannot be changed after a problem is released."
 msgstr ""
 "Thé nümßér öf çrïtérïä çännöt ßé çhängéd äftér ä prößlém ïs réléäséd. Ⱡ'σяєм"
 " ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Criteria names cannot be changed after a problem is released"
 msgstr ""
 "Çrïtérïä nämés çännöt ßé çhängéd äftér ä prößlém ïs réléäséd Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "The number of options cannot be changed after a problem is released."
 msgstr ""
 "Thé nümßér öf öptïöns çännöt ßé çhängéd äftér ä prößlém ïs réléäséd. Ⱡ'σяєм "
 "ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Point values cannot be changed after a problem is released."
 msgstr ""
 "Pöïnt välüés çännöt ßé çhängéd äftér ä prößlém ïs réléäséd. Ⱡ'σяєм ιρѕυм "
 "∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Learner training must have at least one training example."
 msgstr ""
 "Léärnér träïnïng müst hävé ät léäst öné träïnïng éxämplé. Ⱡ'σяєм ιρѕυм ∂σłσя"
 " ѕιт αмєт, ¢σηѕє¢тєтυя α#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "Leaderboard number is invalid."
 msgstr "Léädérßöärd nümßér ïs ïnvälïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
-#: openassessment/xblock/validation.py
+#: xblock/validation.py
 msgid "The submission format is invalid."
 msgstr ""
 "Thé süßmïssïön förmät ïs ïnvälïd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
```

### Comparing `ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -74,14 +74,17 @@
 
 msgid "Demo the new Grading Experience"
 msgstr "Démö thé néw Grädïng Éxpérïénçé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
 
 msgid "Describe "
 msgstr "Désçrïßé  Ⱡ'σяєм ιρѕυм ∂σł#"
 
+msgid "Draft saved!"
+msgstr "Dräft sävéd! Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+
 msgid "Error"
 msgstr "Érrör Ⱡ'σяєм ιρѕ#"
 
 msgid "Error getting the number of ungraded responses"
 msgstr ""
 "Érrör géttïng thé nümßér öf üngrädéd réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
 "¢σηѕє¢тєтυя α#"
@@ -207,14 +210,19 @@
 
 msgid "Peer Responses Received"
 msgstr "Péér Réspönsés Réçéïvéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
 
 msgid "Peers Assessed"
 msgstr "Péérs Àssésséd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
 
+msgid "Please check your internet connection."
+msgstr ""
+"Pléäsé çhéçk ýöür ïntérnét çönnéçtïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
+"¢σηѕє¢тєтυя#"
+
 msgid "Please wait"
 msgstr "Pléäsé wäït Ⱡ'σяєм ιρѕυм ∂σłσя #"
 
 msgid "Preformatted"
 msgstr "Préförmättéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
 
 msgid "Problem cloning rubric"
@@ -222,14 +230,20 @@
 
 msgid "Refresh"
 msgstr "Réfrésh Ⱡ'σяєм ιρѕυм #"
 
 msgid "Save Unsuccessful"
 msgstr "Sävé Ûnsüççéssfül Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
 
+msgid "Saving draft"
+msgstr "Sävïng dräft Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+
+msgid "Saving draft..."
+msgstr "Sävïng dräft... Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
+
 msgid "Saving..."
 msgstr "Sävïng... Ⱡ'σяєм ιρѕυм ∂σł#"
 
 msgid "Self"
 msgstr "Sélf Ⱡ'σяєм ι#"
 
 msgid "Server error."
```

### Comparing `ora2-5.0.4/openassessment/locale/eo/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,695 +1,590 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
-# EdX Team <info@edx.org>, 2018.
-#
+# 
+# Translators:
+# anna.ghetti <anna.ghetti@student.unife.it>, 2014
+# danicabliznakinja <dmbliznakinje@yahoo.co.uk>, 2014
+# Domenico Casanica <domenico.casanica@sistinf.it>, 2021
+# 20bdf6b5822f7ccbe16f09a657dbe357_e29decb, 2021
+# Pietro Lombardo <pietrolombardo1979@gmail.com>, 2015
+# Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021
+# Tiziana Longeri <tiziana.longeri@polimi.it>, 2015
 msgid ""
 msgstr ""
-"Project-Id-Version: edx-ora2\n"
+"Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
-"PO-Revision-Date: 2014-06-04 15:41-0400\n"
-"Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: openedx-translation <openedx-translation@googlegroups.com>\n"
-"Language: eo\n"
+"PO-Revision-Date: 2014-06-11 13:04+0000\n"
+"Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
+"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: it_IT\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
-#: openassessment/xblock/static/js/src/oa_server.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:77
+#: openassessment/xblock/static/js/src/oa_server.js:113
+#: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr ""
-"Thïs séçtïön çöüld nöt ßé löädéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Impossibile caricare questa sezione."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr ""
-"Thé stäff ässéssmént förm çöüld nöt ßé löädéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя α#"
+msgstr "Impossibile caricare il modulo di valutazione dello staff. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
-msgstr ""
-"Thé dïspläý öf üngrädéd änd çhéçkéd öüt réspönsés çöüld nöt ßé löädéd. "
-"Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя #"
+msgstr "Impossibile caricare la visualizzazione delle risposte non valutate e sottoposte a checkout. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr ""
-"Thïs réspönsé çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυ#"
+msgstr "Impossibile inoltrare la risposta."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr ""
-"Thïs réspönsé çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Impossibile salvare la risposta."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr ""
-"Thïs féédßäçk çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυ#"
+msgstr "Impossibile inoltrare il feedback."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
-#: openassessment/xblock/static/js/src/oa_server.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:287
+#: openassessment/xblock/static/js/src/oa_server.js:378
+#: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr ""
-"Thïs ässéssmént çöüld nöt ßé süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя#"
+msgstr "Impossibile inoltrare questa valutazione."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr ""
-"Öné ör möré résçhédülïng täsks fäïléd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя#"
+msgstr "Una o più attività di ripianificazione falite."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr ""
-"Thïs prößlém çöüld nöt ßé sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Impossibile salvare questo problema."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr ""
-"Thé sérvér çöüld nöt ßé çöntäçtéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
+msgstr "Impossibile contattare il server."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Çöüld nöt rétrïévé üplöäd ürl. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
+msgstr "Non si è potuto recuperare l'url dell'upload."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:549
+#: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr "Sérvér érrör. Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
+msgstr "Errore del server. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr ""
-"Çöüld nöt rétrïévé döwnlöäd ürl. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Non si è potuto recuperare l'url del download."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr ""
-"Thé süßmïssïön çöüld nöt ßé rémövéd fröm thé grädïng pööl. Ⱡ'σяєм ιρѕυм "
-"∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α#"
+msgstr "La consegna non ha potuto essere rimossa dal gruppo di classificazione."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
-msgstr ""
-"Mültïplé téäms rétürnéd för çöürsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
+msgstr "Più team restituiti per il corso "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:677
 msgid "Could not load teams information."
-msgstr ""
-"Çöüld nöt löäd téäms ïnförmätïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Impossibile caricare le informazioni sui team. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:699
 msgid "User lookup failed"
-msgstr "Ûsér lööküp fäïléd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
+msgstr "Ricerca utente non riuscita "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:704
 msgid "Error when looking up username"
-msgstr "Érrör whén löökïng üp üsérnämé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
+msgstr "Errore durante la ricerca del nome utente "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/oa_server.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
+#: openassessment/xblock/static/js/src/oa_server.js:728
 msgid "Failed to clone rubric"
-msgstr "Fäïléd tö çlöné rüßrïç Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
+msgstr "Impossibile clonare la rubrica"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "View and grade responses"
-msgstr "Vïéw änd grädé réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
+msgstr "Visualizza e valuta le risposte"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
-msgstr "Démö thé néw Grädïng Éxpérïénçé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
+msgstr "Dimostra la nuova esperienza di valutazione"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
-msgstr "Ûnït Nämé Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Nome unità "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr "Ûnïts Ⱡ'σяєм ιρѕ#"
+msgstr "Unità"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
-msgstr "Àsséssmént Ⱡ'σяєм ιρѕυм ∂σłσ#"
+msgstr "Valutazione"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:106
 msgid "Assessments"
-msgstr "Àsséssménts Ⱡ'σяєм ιρѕυм ∂σłσя #"
+msgstr "Valutazioni "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:113
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:114
 msgid "Total Responses"
-msgstr "Tötäl Réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
+msgstr "Numero totale di risposte "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:121
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:122
 msgid "Training"
-msgstr "Träïnïng Ⱡ'σяєм ιρѕυм ∂#"
+msgstr "Formazione "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:129
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:130
 msgid "Peer"
-msgstr "Péér Ⱡ'σяєм ι#"
+msgstr "Peer"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:137
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:138
 msgid "Self"
-msgstr "Sélf Ⱡ'σяєм ι#"
+msgstr "Autonomo "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:145
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:146
 msgid "Waiting"
-msgstr "Wäïtïng Ⱡ'σяєм ιρѕυм #"
+msgstr "In attesa "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr "Stäff Ⱡ'σяєм ιρѕ#"
+msgstr "Staff"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
-msgstr "Fïnäl Grädé Réçéïvéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, #"
+msgstr "Voto finale ricevuto "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
-msgstr "Stäff Grädér Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+msgstr "Classificatore del personale"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
-msgstr ""
-"Lïst öf Öpén Àsséssménts ïs ünäväïläßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя#"
+msgstr "L'elenco delle valutazioni aperte non è disponibile "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr "Pléäsé wäït Ⱡ'σяєм ιρѕυм ∂σłσя #"
+msgstr "Un attimo, per favore..."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
-msgstr "Blöçk vïéw ïs ünäväïläßlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
+msgstr "Vista blocco non disponibile "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
+#: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
-msgstr "Bäçk tö Füll Lïst Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
+msgstr "Torna all'elenco completo "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
-msgstr "Çönfïrm Ⱡ'σяєм ιρѕυм #"
+msgstr "Conferma"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:7
 msgid "Cancel"
-msgstr "Çänçél Ⱡ'σяєм ιρѕυ#"
+msgstr "Annulla"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
-msgstr ""
-"Ýöür fïlé häs ßéén délétéd ör päth häs ßéén çhängéd:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт"
-" αмєт, ¢σηѕє¢тєтυя α#"
+msgstr "Il tuo file è stato eliminato o il percorso è stato modificato:"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Stätüs öf Ýöür Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
+msgstr "Stato della Tua Risposta"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr ""
-"Thïs réspönsé häs nöt ßéén sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Questa risposta non è stata salvata."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
-msgstr ""
-"Ìf ýöü léävé thïs pägé wïthöüt sävïng ör süßmïttïng ýöür réspönsé, ýöü wïll "
-"lösé äný wörk ýöü hävé döné ön thé réspönsé. Ⱡ'σяєм ιρѕυ#"
+msgstr "Se si esce da questa pagina senza salvare o inoltrare la propria risposta, tutto il lavoro eseguito sulla risposta verrà perso. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Sävïng... Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Salvataggio in corso..."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr ""
-"Thïs réspönsé häs ßéén sävéd ßüt nöt süßmïttéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт,"
-" ¢σηѕє¢тєтυя α#"
+msgstr "Questa risposta è stata salvata, ma non è stata inoltrata."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Érrör Ⱡ'σяєм ιρѕ#"
+msgstr "Errore"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
-msgstr "Çönfïrm Süßmït Réspönsé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
+msgstr "Conferma Invia risposta"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr ""
-"Ýöü'ré äßöüt tö süßmït ýöür réspönsé för thïs ässïgnmént. Àftér ýöü süßmït "
-"thïs réspönsé, ýöü çän't çhängé ït ör süßmït ä néw réspönsé. Ⱡ'σяєм ιρѕυм "
-"∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
-"ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
-"ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
-"¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
-"¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
-"ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт łαвσяυ#"
+msgstr "Stai per inviare la risposta per questo compito. Dopo aver inviato questa risposta, non è possibile modificarla o inviare una nuova risposta."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
-msgstr ""
-"Ìndïvïdüäl fïlé sïzé müst ßé {max_files_mb}MB ör léss. Ⱡ'σяєм ιρѕυм ∂σłσя "
-"ѕιт αмєт, ¢σηѕє¢тєтυя #"
+msgstr "La dimensione del singolo file deve essere uguale o inferiore a {max_files_mb}MB. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:590
 msgid ""
 "File upload failed: unsupported file type. Only the supported file types can"
 " be uploaded. If you have questions, please reach out to the course team."
-msgstr ""
-"Fïlé üplöäd fäïléd: ünsüppörtéd fïlé týpé. Önlý thé süppörtéd fïlé týpés çän"
-" ßé üplöädéd. Ìf ýöü hävé qüéstïöns, pléäsé réäçh öüt tö thé çöürsé téäm. "
-"Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
-"тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
-" qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
-"¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
-"¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
-"ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηι#"
+msgstr "Caricamento del file non riuscito: tipo di file non supportato. È possibile caricare solo i tipi di file supportati. In caso di domande, contattare il team del corso. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
-msgstr ""
-"Thé mäxïmüm nümßér fïlés thät çän ßé sävéd ïs  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя α#"
+msgstr "Il numero massimo di file che è possibile salvare è"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:673
+#: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
-msgstr "Désçrïßé  Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Descrivi "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:673
 msgid "(required):"
-msgstr "(réqüïréd): Ⱡ'σяєм ιρѕυм ∂σłσя #"
+msgstr "(campo obbligatorio)"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
-msgstr "Thümßnäïl vïéw öf  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
+msgstr "Vista miniatura di "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
-msgstr "Çönfïrm Délété Ûplöädéd Fïlé Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
+msgstr "Conferma Elimina file caricato"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_response.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_response.js:805
 msgid ""
 "Are you sure you want to delete the following file? It cannot be restored.\n"
 "File: "
-msgstr ""
-"Àré ýöü süré ýöü wänt tö délété thé föllöwïng fïlé? Ìt çännöt ßé réstöréd.\n"
-"Fïlé:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Si è sicuri di voler eliminare il seguente file? Non sarà possibile ripristinarlo.\nFile: "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_self.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_self.js:138
 msgid ""
 "If you leave this page without submitting your self assessment, you will "
 "lose any work you have done."
-msgstr ""
-"Ìf ýöü léävé thïs pägé wïthöüt süßmïttïng ýöür sélf ässéssmént, ýöü wïll "
-"lösé äný wörk ýöü hävé döné. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
+msgstr "Se si esce da questa pagina senza inoltrare la propria auto-valutazione, tutto il lavoro effettuato verrà perso. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:143
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:253
 msgid "Unexpected server error."
-msgstr "Ûnéxpéçtéd sérvér érrör. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢ση#"
+msgstr "Errore del server non previsto. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:147
 msgid "You must provide a learner name."
-msgstr ""
-"Ýöü müst prövïdé ä léärnér nämé. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "È necessario fornire il nome di uno studente. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:214
 msgid ""
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
-msgstr ""
-"Thïs grädé wïll ßé äpplïéd tö äll mémßérs öf thé téäm. Dö ýöü wänt tö "
-"çöntïnüé? Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
+msgstr "Questo voto verrà applicato a tutti i membri del team. Si desidera continuare? "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
-msgstr "Çönfïrm Grädé Téäm Süßmïssïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
+msgstr "Conferma la presentazione del team di valutazione"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
-msgstr ""
-"Érrör géttïng thé nümßér öf üngrädéd réspönsés Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя α#"
+msgstr "Errore durante l'acquisizione del numero di risposte senza voto "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_staff_area.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_staff_area.js:538
 msgid ""
 "If you leave this page without submitting your staff assessment, you will "
 "lose any work you have done."
-msgstr ""
-"Ìf ýöü léävé thïs pägé wïthöüt süßmïttïng ýöür stäff ässéssmént, ýöü wïll "
-"lösé äný wörk ýöü hävé döné. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
+msgstr "Se si esce d questa pagina senza inoltrare la valutazione dello staff, tutto il lavoro effettuato verrà perso. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_training.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_training.js:130
 msgid "Feedback available for selection."
-msgstr ""
-"Féédßäçk äväïläßlé för séléçtïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тє#"
+msgstr "Feedback disponibile per la selezione. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_peer.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
+#: openassessment/xblock/static/js/src/lms/oa_peer.js:217
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
-msgstr ""
-"Ìf ýöü léävé thïs pägé wïthöüt süßmïttïng ýöür péér ässéssmént, ýöü wïll "
-"lösé äný wörk ýöü hävé döné. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
+msgstr "Se si esce da questa pagina senza inoltrare la valutazione del collega, tutto il lavoro effettuato verrà perso. "
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
-msgstr "Réfrésh Ⱡ'σяєм ιρѕυм #"
+msgstr "Aggiorna"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
-msgstr "Ûsérnämé Ⱡ'σяєм ιρѕυм ∂#"
+msgstr "Nome utente"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peers Assessed"
-msgstr "Péérs Àssésséd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
+msgstr "I pari valutati"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peer Responses Received"
-msgstr "Péér Réspönsés Réçéïvéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σ#"
+msgstr "Risposte dei pari ricevute"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Time Spent On Current Step"
-msgstr "Tïmé Spént Ön Çürrént Stép Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕ#"
+msgstr "Tempo trascorso sul passaggio corrente"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Staff assessment"
-msgstr "Stäff ässéssmént Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αм#"
+msgstr "Valutazione del personale"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Grade Status"
-msgstr "Grädé Stätüs Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+msgstr "Stato del grado"
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "The \"{name}\" problem is configured to require a minimum of {min_grades} "
 "peer grades, and asks to review {min_graded} peers."
-msgstr ""
-"Thé \"{name}\" prößlém ïs çönfïgüréd tö réqüïré ä mïnïmüm öf {min_grades} "
-"péér grädés, änd äsks tö révïéw {min_graded} péérs. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт "
-"αм#"
+msgstr "Il problema &quot;{name}&quot; è configurato per richiedere un minimo di {min_grades} voti peer e chiede di rivedere {min_graded} peer."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "There are currently {stuck_learners} learners in the waiting state, meaning "
 "they have not yet met all requirements for Peer Assessment. "
-msgstr ""
-"Théré äré çürréntlý {stuck_learners} léärnérs ïn thé wäïtïng stäté, méänïng "
-"théý hävé nöt ýét mét äll réqüïréménts för Péér Àsséssmént.  Ⱡ'σяєм ιρ#"
+msgstr "Al momento ci sono {stuck_learners} studenti in stato di attesa, il che significa che non hanno ancora soddisfatto tutti i requisiti per la valutazione tra pari."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "However, {overwritten_count} of these students have received a grade through"
 " the staff grade override tool already."
-msgstr ""
-"Höwévér, {overwritten_count} öf thésé stüdénts hävé réçéïvéd ä grädé thröügh"
-" thé stäff grädé övérrïdé tööl älréädý. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт#"
+msgstr "Tuttavia, {overwritten_count} di questi studenti hanno già ricevuto un voto tramite lo strumento di sostituzione del voto del personale."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
-msgstr ""
-"Érrör whïlé fétçhïng stüdént dätä. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєт#"
+msgstr "Errore durante il recupero dei dati degli studenti."
 
-#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js
-#: openassessment/xblock/static/js/src/lms/oa_base.js
+#: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
+#: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
-msgstr "Ûnäßlé tö löäd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
+msgstr "Impossibile caricare "
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Pärägräph Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Paragrafo"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Préförmättéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+msgstr "Preformattato"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Héädïng 3 Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Titolo 3"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Héädïng 4 Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Titolo 4"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Héädïng 5 Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Titolo 5"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Héädïng 6 Ⱡ'σяєм ιρѕυм ∂σł#"
+msgstr "Titolo 6"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_container_item.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Ûnnäméd Öptïön Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
+msgstr "Opzione senza nome"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_container_item.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Nöt Séléçtéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕ#"
+msgstr "Non Selezionato"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
-msgstr "Prößlém çlönïng rüßrïç Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢#"
+msgstr "Rubrica di clonazione del problema"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr "Çrïtérïön Àddéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт α#"
+msgstr "Criterio aggiunto"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
-msgstr ""
-"Ýöü hävé äddéd ä çrïtérïön. Ýöü wïll nééd tö séléçt än öptïön för thé "
-"çrïtérïön ïn thé Léärnér Träïnïng stép. Tö dö thïs, çlïçk thé Àsséssmént "
-"Stéps täß. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ"
-" єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ "
-"мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ "
-"єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє "
-"νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт "
-"¢υρι∂αтαт ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłι#"
-
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+msgstr "Hai aggiunto un criterio. Dovrai selezionare un&#39;opzione per il criterio nella fase di formazione dello studente. Per fare ciò, fare clic sulla scheda Passi di valutazione."
+
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Öptïön Délétéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт#"
+msgstr "Opzione cancellata"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr ""
-"Ýöü hävé délétéd än öptïön. Thät öptïön häs ßéén rémövéd fröm ïts çrïtérïön "
-"ïn thé sämplé réspönsés ïn thé Léärnér Träïnïng stép. Ýöü mïght hävé tö "
-"séléçt ä néw öptïön för thé çrïtérïön. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт "
-"∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση "
-"υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ ¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє "
-"∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє ¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα"
-" ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт ηση ρяσι∂є#"
+msgstr "È stata eliminata un'opzione. Questa opzione è stata rimossa dal relativo criterio nelle risposte di esempio nella fase Addestramento studente. Potrebbe essere necessario selezionare una nuova opzione per il criterio. "
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr ""
-"Ýöü hävé délétéd äll thé öptïöns för thïs çrïtérïön. Thé çrïtérïön häs ßéén "
-"rémövéd fröm thé sämplé réspönsés ïn thé Léärnér Träïnïng stép. Ⱡ'σяєм ιρѕυм"
-" ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ тємρσя "
-"ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм, qυιѕ "
-"ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
-"¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
-"¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
-"ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт αηιм ι∂ єѕт łα#"
+msgstr "Tutte le opzioni per questo criterio sono state eliminate. Il criterio è stato rimosso dalle risposte di esempio nella fase Addestramento studente. "
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr "Çrïtérïön Délétéd Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
+msgstr "Criterio cancellato"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr ""
-"Ýöü hävé délétéd ä çrïtérïön. Thé çrïtérïön häs ßéén rémövéd fröm thé "
-"éxämplé réspönsés ïn thé Léärnér Träïnïng stép. Ⱡ'σяєм ιρѕυм ∂#"
+msgstr "È stato eliminato un criterio. Il criterio è stato rimosso dalle risposte di esempio nella fase Addestramento studente. "
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Wärnïng Ⱡ'σяєм ιρѕυм #"
+msgstr "Allerta"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr ""
-"Çhängés tö stéps thät äré nöt séléçtéd äs pärt öf thé ässïgnmént wïll nöt ßé"
-" sävéd. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢т#"
+msgstr "Le modifiche ai passaggi che non sono selezionati come parte del compito non verranno salvate."
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr "Fïlé týpés çän nöt ßé émptý. Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢#"
+msgstr "I tipi di file non possono essere vuoti. "
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr ""
-"Thé föllöwïng fïlé týpés äré nöt ällöwéd:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя #"
+msgstr "I seguenti tipi di file non sono ammessi:"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
-msgstr "Sävé Ûnsüççéssfül Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмє#"
+msgstr "Salvataggio non riuscito"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
-msgstr ""
-"Érrörs détéçtéd ön thé föllöwïng täßs:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, "
-"¢σηѕє¢тєтυя#"
+msgstr "Errori rilevati nelle seguenti schede:"
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 msgid ""
 "This ORA has already been released. Changes will only affect learners making"
 " new submissions. Existing submissions will not be modified by this change."
-msgstr ""
-"Thïs ÖRÀ häs älréädý ßéén réléäséd. Çhängés wïll önlý äfféçt léärnérs mäkïng"
-" néw süßmïssïöns. Éxïstïng süßmïssïöns wïll nöt ßé mödïfïéd ßý thïs çhängé. "
-"Ⱡ'σяєм ιρѕυм ∂σłσя ѕιт αмєт, ¢σηѕє¢тєтυя α∂ιριѕι¢ιηg єłιт, ѕє∂ ∂σ єιυѕмσ∂ "
-"тємρσя ιη¢ι∂ι∂υηт υт łαвσяє єт ∂σłσяє мαgηα αłιqυα. υт єηιм α∂ мιηιм νєηιαм,"
-" qυιѕ ησѕтяυ∂ єχєя¢ιтαтιση υłłαм¢σ łαвσяιѕ ηιѕι υт αłιqυιρ єχ єα ¢σммσ∂σ "
-"¢σηѕєqυαт. ∂υιѕ αυтє ιяυяє ∂σłσя ιη яєρяєнєη∂єяιт ιη νσłυρтαтє νєłιт єѕѕє "
-"¢ιłłυм ∂σłσяє єυ ƒυgιαт ηυłłα ραяιαтυя. єχ¢єρтєυя ѕιηт σ¢¢αє¢αт ¢υρι∂αтαт "
-"ηση ρяσι∂єηт, ѕυηт ιη ¢υłρα qυι σƒƒι¢ια ∂єѕєяυηт мσłłιт α#"
+msgstr "Questo ORA è già stato rilasciato. Le modifiche riguarderanno solo gli studenti che effettuano nuovi invii. Gli invii esistenti non verranno modificati da questa modifica."
 
-#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js
-#: openassessment/xblock/static/js/src/studio/oa_edit.js
+#: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
+#: openassessment/xblock/static/js/src/studio/oa_edit.js:318
 msgid "error count: "
-msgstr "érrör çöünt:  Ⱡ'σяєм ιρѕυм ∂σłσя ѕι#"
+msgstr "conteggio errori:"
```

### Comparing `ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_419/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/he/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/hi/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/id/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,590 +1,600 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# anna.ghetti <anna.ghetti@student.unife.it>, 2014
-# danicabliznakinja <dmbliznakinje@yahoo.co.uk>, 2014
-# Domenico Casanica <domenico.casanica@sistinf.it>, 2021
-# 20bdf6b5822f7ccbe16f09a657dbe357_e29decb, 2021
-# Pietro Lombardo <pietrolombardo1979@gmail.com>, 2015
-# Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021
-# Tiziana Longeri <tiziana.longeri@polimi.it>, 2015
+# Beatriz Magalhães <mbeatrizmagalhaes@gmail.com>, 2016
+# Beatriz Sousa <beatriz.sousa@bridgelk.com>, 2018
+# Cátia Lopes <catia.lopes@bridgelk.com>, 2018
+# Filipa Macieira <filipa.macieira@fccn.pt>, 2021
+# Filipe Boleto <fboleto@gmail.com>, 2015
+# Ivo Branco <ivo.branco@fccn.pt>, 2023
+# Luis Manuel Moreno <luis.moreno@edunext.co>, 2019
+# Manuela Silva <mmsrs@sky.com>, 2016,2018
+# Manuela Silva <mmsrs@sky.com>, 2018
+# Manuela Silva <mmsrs@sky.com>, 2016
+# MS, 2016,2018
+# Nika Shahidian, 2022
+# Nlaranjo <numicola@gmail.com>, 2014
+# Nlaranjo <numicola@gmail.com>, 2014
+# Rui Ribeiro <info@nau.edu.pt>, 2019
+# Rui Ribeiro <info@nau.edu.pt>, 2019
+# Teresa Guerreiro <t.guerreiro@sapo.pt>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
-"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
+"Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2023\n"
+"Language-Team: Portuguese (Portugal) (http://app.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: it_IT\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: pt_PT\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Impossibile caricare questa sezione."
+msgstr "Não foi possível carregar esta secção."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr "Impossibile caricare il modulo di valutazione dello staff. "
+msgstr "Não foi possível carregar o formulário de avaliação da Equipa."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
-msgstr "Impossibile caricare la visualizzazione delle risposte non valutate e sottoposte a checkout. "
+msgstr "Não foi possível carregar a exibição de respostas entregues não classificadas."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Impossibile inoltrare la risposta."
+msgstr "Não foi possível submeter esta resposta."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Impossibile salvare la risposta."
+msgstr "Não foi possível guardar esta resposta."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Impossibile inoltrare il feedback."
+msgstr "Não foi possível submeter este comentário."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Impossibile inoltrare questa valutazione."
+msgstr "Não foi possível submeter esta avaliação."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Una o più attività di ripianificazione falite."
+msgstr "Ocorreu erro no reagendamento de uma ou mais tarefas."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Impossibile salvare questo problema."
+msgstr "Não foi possível gravar este problema."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Impossibile contattare il server."
+msgstr "Não foi possível contactar o servidor."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Non si è potuto recuperare l'url dell'upload."
+msgstr "Não foi possível recuperar o url de envio."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr "Errore del server. "
+msgstr "Erro de servidor."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "Non si è potuto recuperare l'url del download."
+msgstr "Não foi possível obter os dados a partir do URL definido."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr "La consegna non ha potuto essere rimossa dal gruppo di classificazione."
+msgstr "Não foi possível remover a submissão da pool de classificação."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
-msgstr "Più team restituiti per il corso "
+msgstr "Várias equipas voltaram para o curso"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:677
 msgid "Could not load teams information."
-msgstr "Impossibile caricare le informazioni sui team. "
+msgstr "Não foi possível carregar informação das equipas."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:699
 msgid "User lookup failed"
-msgstr "Ricerca utente non riuscita "
+msgstr "A procura do utilizador falhou"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:704
 msgid "Error when looking up username"
-msgstr "Errore durante la ricerca del nome utente "
+msgstr "Erro ao procurar o nome de utilizador"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:728
 msgid "Failed to clone rubric"
-msgstr "Impossibile clonare la rubrica"
+msgstr "Falha na clonagem da rubrica"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "View and grade responses"
-msgstr "Visualizza e valuta le risposte"
+msgstr "Ver e classificar as respostas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
-msgstr "Dimostra la nuova esperienza di valutazione"
+msgstr "Demonstração da nova experiência de classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
-msgstr "Nome unità "
+msgstr "Título da Unidade"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr "Unità"
+msgstr "Unidades"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
-msgstr "Valutazione"
+msgstr "Avaliação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:106
 msgid "Assessments"
-msgstr "Valutazioni "
+msgstr "Avaliações"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:113
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:114
 msgid "Total Responses"
-msgstr "Numero totale di risposte "
+msgstr "Total de Respostas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:121
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:122
 msgid "Training"
-msgstr "Formazione "
+msgstr "Formação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:129
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:130
 msgid "Peer"
-msgstr "Peer"
+msgstr "Par"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:137
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:138
 msgid "Self"
-msgstr "Autonomo "
+msgstr "Auto"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:145
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:146
 msgid "Waiting"
-msgstr "In attesa "
+msgstr "A aguardar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr "Staff"
+msgstr "Equipa"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
-msgstr "Voto finale ricevuto "
+msgstr "Nota Final Recebida"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
-msgstr "Classificatore del personale"
+msgstr "Graduador de Pessoal"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
-msgstr "L'elenco delle valutazioni aperte non è disponibile "
+msgstr "Lista de Avaliações Abertas não está disponível"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr "Un attimo, per favore..."
+msgstr "Aguarde, por favor"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
-msgstr "Vista blocco non disponibile "
+msgstr "A visualização em grelha não está disponível"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
-msgstr "Torna all'elenco completo "
+msgstr "Voltar à lista completa"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
-msgstr "Conferma"
+msgstr "Confirmar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:7
 msgid "Cancel"
-msgstr "Annulla"
+msgstr "Cancelar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
-msgstr "Il tuo file è stato eliminato o il percorso è stato modificato:"
+msgstr "O seu ficheiro foi eliminado ou o caminho foi alterado: "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Stato della Tua Risposta"
+msgstr "Estado da sua Resposta"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Questa risposta non è stata salvata."
+msgstr "Esta resposta não foi guardada."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
-msgstr "Se si esce da questa pagina senza salvare o inoltrare la propria risposta, tutto il lavoro eseguito sulla risposta verrà perso. "
+msgstr "Caso saia desta página sem gravar ou submeter a sua resposta, irá perder todo o trabalho até aqui realizado."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Salvataggio in corso..."
+msgstr "A guardar..."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Questa risposta è stata salvata, ma non è stata inoltrata."
+msgstr "Esta resposta foi guardada mas não foi submetida."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Errore"
+msgstr "Erro"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
-msgstr "Conferma Invia risposta"
+msgstr "Confirmar Submissão da Resposta"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr "Stai per inviare la risposta per questo compito. Dopo aver inviato questa risposta, non è possibile modificarla o inviare una nuova risposta."
+msgstr "Está prestes a submeter a sua resposta para esta tarefa. Depois de a submeter, não é possível alterá-la ou submeter uma nova resposta."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
-msgstr "La dimensione del singolo file deve essere uguale o inferiore a {max_files_mb}MB. "
+msgstr "O tamanho do ficheiro individual deve ser {max_files_mb}MB ou menos."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:590
 msgid ""
 "File upload failed: unsupported file type. Only the supported file types can"
 " be uploaded. If you have questions, please reach out to the course team."
-msgstr "Caricamento del file non riuscito: tipo di file non supportato. È possibile caricare solo i tipi di file supportati. In caso di domande, contattare il team del corso. "
+msgstr "Falha no carregamento do ficheiro: tipo de ficheiro não suportado. Apenas os tipos de ficheiros suportados podem ser carregados. Se tiver dúvidas, entre em contato com a equipa de curso."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
-msgstr "Il numero massimo di file che è possibile salvare è"
+msgstr "O número máximo de ficheiros que podem ser guardados é "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 #: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
-msgstr "Descrivi "
+msgstr "Descreva "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 msgid "(required):"
-msgstr "(campo obbligatorio)"
+msgstr "(obrigatório):"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
-msgstr "Vista miniatura di "
+msgstr "Visualização em miniatura de "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
-msgstr "Conferma Elimina file caricato"
+msgstr "Confirmar exclusão do arquivo enviado"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:805
 msgid ""
 "Are you sure you want to delete the following file? It cannot be restored.\n"
 "File: "
-msgstr "Si è sicuri di voler eliminare il seguente file? Non sarà possibile ripristinarlo.\nFile: "
+msgstr "Tem certeza de que deseja apagar o seguinte ficheiro? Não pode ser restaurado.\nFicheiro: "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_self.js:138
 msgid ""
 "If you leave this page without submitting your self assessment, you will "
 "lose any work you have done."
-msgstr "Se si esce da questa pagina senza inoltrare la propria auto-valutazione, tutto il lavoro effettuato verrà perso. "
+msgstr "Caso saia desta página sem submeter a sua auto-avaliação, irá perder todo o trabalho até aqui realizado."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:143
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:253
 msgid "Unexpected server error."
-msgstr "Errore del server non previsto. "
+msgstr "Erro do servidor."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:147
 msgid "You must provide a learner name."
-msgstr "È necessario fornire il nome di uno studente. "
+msgstr "Deve indicar o nome de um estudante."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:214
 msgid ""
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
-msgstr "Questo voto verrà applicato a tutti i membri del team. Si desidera continuare? "
+msgstr "Esta nota será aplicada a todos os membros da equipa. Quer continuar?"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
-msgstr "Conferma la presentazione del team di valutazione"
+msgstr "Confirme o envio da equipe de notas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
-msgstr "Errore durante l'acquisizione del numero di risposte senza voto "
+msgstr "Erro ao obter o número de respostas sem classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:538
 msgid ""
 "If you leave this page without submitting your staff assessment, you will "
 "lose any work you have done."
-msgstr "Se si esce d questa pagina senza inoltrare la valutazione dello staff, tutto il lavoro effettuato verrà perso. "
+msgstr "Caso saia desta página sem submeter a sua avaliação individual, irá perder todo o trabalho até aqui realizado."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_training.js:130
 msgid "Feedback available for selection."
-msgstr "Feedback disponibile per la selezione. "
+msgstr "Comentário disponível para a seleção."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_peer.js:217
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
-msgstr "Se si esce da questa pagina senza inoltrare la valutazione del collega, tutto il lavoro effettuato verrà perso. "
+msgstr "Caso saia desta página sem submeter o seu teste, irá perder todo o trabalho até aqui realizado."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
-msgstr "Aggiorna"
+msgstr "Atualizar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
-msgstr "Nome utente"
+msgstr "Nome de utilizador"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peers Assessed"
-msgstr "I pari valutati"
+msgstr "Colegas avaliados"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peer Responses Received"
-msgstr "Risposte dei pari ricevute"
+msgstr "Respostas de Colegas Recebidas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Time Spent On Current Step"
-msgstr "Tempo trascorso sul passaggio corrente"
+msgstr "Tempo Gasto Na Etapa Atual"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Staff assessment"
-msgstr "Valutazione del personale"
+msgstr "Avaliação da equipa"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Grade Status"
-msgstr "Stato del grado"
+msgstr "Estado da Classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "The \"{name}\" problem is configured to require a minimum of {min_grades} "
 "peer grades, and asks to review {min_graded} peers."
-msgstr "Il problema &quot;{name}&quot; è configurato per richiedere un minimo di {min_grades} voti peer e chiede di rivedere {min_graded} peer."
+msgstr "O problema \"{name}\" está configurado para exigir um mínimo de {min_grades} avaliações de colegas, e pede para rever {min_graded} colegas."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "There are currently {stuck_learners} learners in the waiting state, meaning "
 "they have not yet met all requirements for Peer Assessment. "
-msgstr "Al momento ci sono {stuck_learners} studenti in stato di attesa, il che significa che non hanno ancora soddisfatto tutti i requisiti per la valutazione tra pari."
+msgstr "Existem atualmente {stuck_learners} estudantes no estado de espera, o que significa que ainda não cumpriram todos os requisitos para a Avaliação por Colegas. "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "However, {overwritten_count} of these students have received a grade through"
 " the staff grade override tool already."
-msgstr "Tuttavia, {overwritten_count} di questi studenti hanno già ricevuto un voto tramite lo strumento di sostituzione del voto del personale."
+msgstr "No entanto, {overwritten_count} destes estudantes já receberam uma classificação através da ferramenta de substituição de classificações da equipa."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
-msgstr "Errore durante il recupero dei dati degli studenti."
+msgstr "Erro ao ir buscar dados de estudantes."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
-msgstr "Impossibile caricare "
+msgstr "Não foi possível carregar"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Paragrafo"
+msgstr "Parágrafo"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Preformattato"
+msgstr "Pré-formatado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Titolo 3"
+msgstr "Título 3"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Titolo 4"
+msgstr "Título 4"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Titolo 5"
+msgstr "Título 5"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Titolo 6"
+msgstr "Título 6"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Opzione senza nome"
+msgstr "Opção sem título"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Non Selezionato"
+msgstr "Não Selecionado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
-msgstr "Rubrica di clonazione del problema"
+msgstr "Rúbrica de clonagem de problemas"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr "Criterio aggiunto"
+msgstr "Critério Adicionado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
-msgstr "Hai aggiunto un criterio. Dovrai selezionare un&#39;opzione per il criterio nella fase di formazione dello studente. Per fare ciò, fare clic sulla scheda Passi di valutazione."
+msgstr "Adicionou um critério. Terá de selecionar uma opção para o critério na etapa de Formação do Estudante. Para o fazer, clique no separador Passos de Avaliação."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Opzione cancellata"
+msgstr "Opção eliminada"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr "È stata eliminata un'opzione. Questa opzione è stata rimossa dal relativo criterio nelle risposte di esempio nella fase Addestramento studente. Potrebbe essere necessario selezionare una nuova opzione per il criterio. "
+msgstr "Eliminou uma opção. Esta opção foi removida do seu critério nos exemplos de respostas da etapa Formação do Estudante. Deve selecionar uma nova opção para esse critério."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr "Tutte le opzioni per questo criterio sono state eliminate. Il criterio è stato rimosso dalle risposte di esempio nella fase Addestramento studente. "
+msgstr "Eliminou todas as opções para este critério. O critério foi removido dos exemplos de resposta da etapa de Formação do Estudante."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr "Criterio cancellato"
+msgstr "Critério eliminado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr "È stato eliminato un criterio. Il criterio è stato rimosso dalle risposte di esempio nella fase Addestramento studente. "
+msgstr "Eliminou um critério. O critério foi removido dos exemplos de resposta da etapa de Formação do Estudante."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Allerta"
+msgstr "Aviso"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr "Le modifiche ai passaggi che non sono selezionati come parte del compito non verranno salvate."
+msgstr "As alterações às etapas que não estão selecionados como parte da tarefa, não serão guardadas."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr "I tipi di file non possono essere vuoti. "
+msgstr "O tipo de ficheiro não pode estar vazio."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr "I seguenti tipi di file non sono ammessi:"
+msgstr "Os seguintes tipos de ficheiro não são permitidos: "
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
-msgstr "Salvataggio non riuscito"
+msgstr "Sem Sucesso ao Guardar"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
-msgstr "Errori rilevati nelle seguenti schede:"
+msgstr "Erros detetados nos seguintes separadores: "
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 msgid ""
 "This ORA has already been released. Changes will only affect learners making"
 " new submissions. Existing submissions will not be modified by this change."
-msgstr "Questo ORA è già stato rilasciato. Le modifiche riguarderanno solo gli studenti che effettuano nuovi invii. Gli invii esistenti non verranno modificati da questa modifica."
+msgstr "Esta Questão de Resposta Aberta já foi divulgada. As alterações apenas irão afetar os alunos que fizerem novas submissões. As submissões existentes não serão modificadas por esta alteração."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:318
 msgid "error count: "
-msgstr "conteggio errori:"
+msgstr "contagem de erros: "
```

### Comparing `ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ka/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/lv/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,109 +1,113 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
+# Alexandra <elenadintroia1986@yahoo.com>, 2015
+# Alex Coman <itsalexcoman@gmail.com>, 2019
+# Irina Maria Curuia, 2015
+# Manuel, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/language/lv/)\n"
+"Last-Translator: Manuel, 2021\n"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: lv\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : 2);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr ""
+msgstr "Această secţiune nu a putut fi încărcată."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr ""
+msgstr "Formularul de evaluare a personalului nu a putut fi încărcat."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr ""
+msgstr "Acest răspuns nu a putut fi trimis."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr ""
+msgstr "Acest răspuns nu a putut fi salvat."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr ""
+msgstr "Feedback-ul nu a putut fi trimis."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr ""
+msgstr "Această evaluare nu a putut fi trimisă."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr ""
+msgstr "Una sau mai multe reprogramări au eşuat."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr ""
+msgstr "Această problemă nu a putut fi salvată."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr ""
+msgstr "Serverul nu a putut fi contactat."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr ""
+msgstr "Nu s-a putut obţine linkul de încărcare."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr ""
+msgstr "Eroare de server."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr ""
+msgstr "Nu s-a putut obţine linkul de descărcare."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
 msgstr ""
 
@@ -151,15 +155,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr "Aktivitātes"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -197,15 +201,15 @@
 msgid "Waiting"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr "Personāls"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
 msgstr ""
 
@@ -219,15 +223,15 @@
 msgid "List of Open Assessments is unavailable"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr "Lūdzu, uzgaidiet"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -249,42 +253,42 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr ""
+msgstr "Statusul răspunsului tău"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr ""
+msgstr "Acest răspuns nu a fost salvat."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr ""
+msgstr "Se salvează..."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr ""
+msgstr "Acest răspuns a fost salvat, dar nu și trimis."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Kļūda"
+msgstr "Eroare"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -447,50 +451,50 @@
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Paragrāfs"
+msgstr "Paragraf"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Iepriekš formatēts"
+msgstr "Preformatat"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Virsraksts 3"
+msgstr "Titlu 3"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Virsraksts 4"
+msgstr "Titlu 4"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Virsraksts 5"
+msgstr "Titlu 5"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Virsraksts 6"
+msgstr "Titlu 6"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Nav izvēlēts"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
```

### Comparing `ora2-5.0.4/openassessment/locale/messages.mo` & `ora2-5.1.0/openassessment/locale/messages.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Buyandelger Batbayar <buyka.1776@gmail.com>, 2021
-# Jamka Sukhee <jambka.93@gmail.com>, 2021
-# Mendbayar Gantulga <mendbayar_mgo@yahoo.com>, 2021
-# Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021
+# Bogdan Mateescu, 2018
+# Pinman <bogdan.stefan@outlook.com>, 2014
+# Rares Mihai Popa <raresmihaipopa@gmail.com>, 2015
+# tyby94 <tyby04@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021\n"
-"Language-Team: Mongolian (http://app.transifex.com/open-edx/edx-platform/language/mn/)\n"
+"Last-Translator: Bogdan Mateescu, 2018\n"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: mn\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
@@ -145,35 +145,35 @@
 
 #: openassessment/data.py:1320
 msgid "No description provided."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:28
 msgid "Save"
-msgstr ""
+msgstr "Salvează"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
-msgstr ""
+msgstr "Anulează"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:5
 msgid "Display Name "
-msgstr ""
+msgstr "Nume afisat"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:8
 msgid "The display name for this component."
-msgstr ""
+msgstr "Numele afișat pentru acest element."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:12
 msgid "Text Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:20
 msgid ""
@@ -215,15 +215,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:53
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:94
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:132
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:158
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:46
 msgid "True"
-msgstr ""
+msgstr "Adevarat"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:56
 msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
@@ -327,15 +327,15 @@
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:9
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:7
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:10
 msgid "Remove"
-msgstr ""
+msgstr "Inlatura"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:17
 msgid "Criterion Name"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:29
 msgid "Criterion Prompt"
@@ -348,58 +348,58 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:52
 msgid "Feedback for This Criterion"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:54
 #: openassessment/xblock/studio_mixin.py:49
 msgid "None"
-msgstr ""
+msgstr "Nimic"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:55
 #: openassessment/xblock/studio_mixin.py:48
 msgid "Optional"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:56
 #: openassessment/templates/openassessmentblock/oa_rubric.html:13
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:93
 #: openassessment/xblock/studio_mixin.py:47
 msgid "Required"
-msgstr ""
+msgstr "Necesar"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:61
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:3
 msgid "Open Response Assessment"
-msgstr "Нээлттэй хариулах асуултын үнэлгээ"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:8
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:7
 msgid "Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:15
 msgid "Rubric"
-msgstr ""
+msgstr "Rubrica"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:22
 msgid "Schedule"
-msgstr ""
+msgstr "Program"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr "Тохиргоо"
+msgstr "Setări"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
@@ -468,30 +468,30 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:5
 msgid "Peer Assessment Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:10
 msgid "Start Date"
-msgstr ""
+msgstr "Data de început"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:19
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:19
 msgid "Start Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:119
 msgid "Due Date"
-msgstr ""
+msgstr "Data Scadentă"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:40
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:40
 msgid "Due Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:48
@@ -673,25 +673,25 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr "Хариулт"
+msgstr "Răspuns:"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
-msgstr ""
+msgstr "Nu a fost Selectat"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:128
 msgid "points"
-msgstr ""
+msgstr "puncte"
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
@@ -703,30 +703,31 @@
 "\n"
 "                      %(assessment_title)s - %(points)s point\n"
 "                  "
 msgid_plural ""
 "\n"
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "\n                      %(assessment_title)s - %(points)s punct\n                  "
+msgstr[1] "\n                      %(assessment_title)s - %(points)s puncte\n                  "
+msgstr[2] "\n                      %(assessment_title)s - %(points)s de puncte\n                  "
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:24
 #, python-format
 msgid "More information about %(name)s"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
 msgid "Your Grade"
-msgstr "Таны Оноо"
+msgstr "Nota dvs."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:19
 #, python-format
 msgid ""
 "\n"
 "                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
@@ -743,23 +744,23 @@
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr "Таны хариулт"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
-msgstr "Таны хариултын үнэлгээ"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:50
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:132
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:28
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:28
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:4
 #: openassessment/templates/openassessmentblock/message/oa_message_closed.html:4
@@ -773,15 +774,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:31
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:29
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:25
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:30
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:27
 msgid "Status"
-msgstr ""
+msgstr "Status"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:65
 msgid "Overall Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:70
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:28
@@ -849,15 +850,15 @@
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr "Дуусаагүй"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
@@ -890,15 +891,15 @@
 msgid ""
 "Grade Available Responses is unavailable. This item is not configured for "
 "Staff Assessment."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html:6
 msgid "Please wait"
-msgstr ""
+msgstr "Vă rugăm așteptați"
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:15
 msgid "Waiting Step Details"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:24
 msgid ""
@@ -1070,15 +1071,15 @@
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
-msgstr ""
+msgstr "Se încarcă"
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
 msgid "Preview in LaTeX"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:10
 msgid "Click to preview your submission in LaTeX."
@@ -1086,19 +1087,19 @@
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:15
 msgid "Preview Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
-msgstr ""
+msgstr "Comentarii"
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
-msgstr "Энэ хэсгийн асуулт"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:27
 #: openassessment/templates/openassessmentblock/oa_uploaded_file.html:34
@@ -1178,15 +1179,15 @@
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html:19
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:21
 #: openassessment/templates/openassessmentblock/self/oa_self_cancelled.html:21
 #: openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html:18
 #: openassessment/xblock/staff_assessment_mixin.py:172
 msgid "Cancelled"
-msgstr ""
+msgstr "Anulat"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html:20
 #, python-format
 msgid ""
 "\n"
 "            Incomplete (%(num_graded)s of %(num_must_grade)s)\n"
 "        "
@@ -1197,15 +1198,15 @@
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr "Гүйцээсэн"
+msgstr "Completat"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
@@ -1285,15 +1286,15 @@
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
-msgstr ""
+msgstr "În Progres"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
@@ -1372,15 +1373,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:244
 msgid "(Required)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:175
 #: openassessment/templates/openassessmentblock/response/oa_response.html:246
 msgid "(Optional)"
-msgstr ""
+msgstr "(Optional)"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:179
 msgid ""
 "\n"
 "                                              Teams should designate one team member to submit a response on behalf of the\n"
 "                                              entire team.  All team members can use this space to work on draft responses,\n"
 "                                              but you will not be able to see your teammates' drafts made in this space, so\n"
@@ -1529,15 +1530,15 @@
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:19
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:20
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
-msgstr ""
+msgstr "Incomplet"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
@@ -1546,15 +1547,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:20
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:20
 #: openassessment/templates/openassessmentblock/self/oa_self_complete.html:18
 #: openassessment/templates/openassessmentblock/student_training/student_training_complete.html:17
 #: openassessment/xblock/staff_assessment_mixin.py:179
 #: openassessment/xblock/staff_assessment_mixin.py:202
 msgid "Complete"
-msgstr ""
+msgstr "Complet"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:51
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:57
 msgid "Your response"
 msgstr ""
 
@@ -1591,30 +1592,30 @@
 "\n"
 "                        You still need to complete the %(start_tag)sself assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:15
 msgid "Error"
-msgstr ""
+msgstr "Eroare"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:29
 #, python-format
 msgid ""
 "\n"
 "                            You joined Team %(team_name)s after they submitted a response for this assignment\n"
 "                            and you will not receive a grade for their response. You have also not previously submitted\n"
 "                            a response to this assignment with another team. Please contact course staff to discuss your\n"
 "                            options for this assignment.\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:23
 msgid "Assess Your Response"
-msgstr "Таны хариултын үнэлгээ"
+msgstr ""
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:31
 #, python-format, python-brace-format
 msgid ""
@@ -1672,15 +1673,15 @@
 msgid "View ORA in Studio"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:69
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:151
 msgid "Close"
-msgstr ""
+msgstr "Închide"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:37
 msgid "Manage Teams"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:50
 msgid "Enter an individual learner's username or email"
@@ -1688,23 +1689,23 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:52
 msgid "Enter a team member's username or edX email"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:56
 msgid "Submit"
-msgstr ""
+msgstr "Trimite"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:78
 msgid "Response total"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:84
 msgid "Location"
-msgstr ""
+msgstr "Locație"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:90
 msgid "Learner Progress"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:94
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:117
@@ -1722,15 +1723,15 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:118
 msgid "Release Date"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:131
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:137
 msgid "N/A"
-msgstr ""
+msgstr "N/A"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
@@ -1771,15 +1772,15 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:57
 msgid "The learner's response to the prompt above"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:64
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:57
 msgid "Submit assessment"
-msgstr ""
+msgstr "Trimite evaluarea"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:70
 msgid "Submit assessment and continue grading"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html:6
 #, python-format
@@ -1884,15 +1885,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:112
 #, python-format
 msgid ""
 "\n"
 "                            Final grade: %(points_earned)s out of %(points_possible)s\n"
 "                        "
-msgstr "\nЭцсийн үнэлгээ: %(points_possible)s онооноос %(points_earned)s"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:119
 msgid "Final Grade Details"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:139
 #, python-format
@@ -1902,14 +1903,15 @@
 "                                    "
 msgid_plural ""
 "\n"
 "                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:165
 msgid "The submission is waiting for assessments."
@@ -2012,15 +2014,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:26
 msgid "Selected Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
-msgstr "Санал шүүмж"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
@@ -2178,15 +2180,15 @@
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Self Assessment Grade"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Your Self Assessment"
-msgstr "Таны өөрийгөө үнэлэх үнэлгээ"
+msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:385
 #: openassessment/xblock/grade_mixin.py:527
 msgid "Your Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:481
@@ -2212,15 +2214,15 @@
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:662
 #, python-brace-format
 msgid ""
 "You have successfully completed this problem and received a "
 "{earned_points}/{total_points}."
-msgstr "Та энэ дасгалыг амжилттай дуусгаж {earned_points}/{total_points} оноо авлаа."
+msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:670
 msgid ""
 "You have not yet received all necessary peer reviews to determine your final"
 " grade."
 msgstr ""
 
@@ -2526,15 +2528,15 @@
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:261
 msgid "This response could not be saved."
-msgstr ""
+msgstr "Acest raspuns nu poate fi salvat."
 
 #: openassessment/xblock/submission_mixin.py:265
 msgid "This response was not submitted."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:281
 msgid "Files descriptions were not submitted."
@@ -2560,19 +2562,19 @@
 
 #: openassessment/xblock/submission_mixin.py:508
 msgid "Error retrieving upload URL."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:790
 msgid "This response has been saved but not submitted."
-msgstr ""
+msgstr "Acest răspuns a fost salvat dar nu trimis."
 
 #: openassessment/xblock/submission_mixin.py:791
 msgid "This response has not been saved."
-msgstr ""
+msgstr "Răspunsul nu a fost salvat."
 
 #: openassessment/xblock/validation.py:118
 msgid "This problem must include at least one assessment."
 msgstr ""
 
 #: openassessment/xblock/validation.py:122
 msgid "The assessment order you selected is invalid."
```

### Comparing `ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/mn/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/nb/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pl/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,600 +1,592 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Beatriz Magalhães <mbeatrizmagalhaes@gmail.com>, 2016
-# Beatriz Sousa <beatriz.sousa@bridgelk.com>, 2018
-# Cátia Lopes <catia.lopes@bridgelk.com>, 2018
-# Filipa Macieira <filipa.macieira@fccn.pt>, 2021
-# Filipe Boleto <fboleto@gmail.com>, 2015
-# Ivo Branco <ivo.branco@fccn.pt>, 2023
-# Luis Manuel Moreno <luis.moreno@edunext.co>, 2019
-# Manuela Silva <mmsrs@sky.com>, 2016,2018
-# Manuela Silva <mmsrs@sky.com>, 2018
-# Manuela Silva <mmsrs@sky.com>, 2016
-# MS, 2016,2018
-# Nika Shahidian, 2022
-# Nlaranjo <numicola@gmail.com>, 2014
-# Nlaranjo <numicola@gmail.com>, 2014
-# Rui Ribeiro <info@nau.edu.pt>, 2019
-# Rui Ribeiro <info@nau.edu.pt>, 2019
-# Teresa Guerreiro <t.guerreiro@sapo.pt>, 2014
+# Adem Özgür <admozgur@gmail.com>, 2015
+# Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022
+# ali selek <aliselek01@gmail.com>, 2015
+# Emrah Emirtekin <eemirtekin@gmail.com>, 2015
+# Hakan Şenel <hgsenel@gmail.com>, 2017
+# İlker IŞIK <m.ilkerisik@hotmail.com>, 2015-2016
+# Kubilay <kubilayinceoren10@gmail.com>, 2015
+# msare <mervesareakin@gmail.com>, 2014
+# Zeynep Ozdemir <gzeynepozdemir@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2023\n"
-"Language-Team: Portuguese (Portugal) (http://app.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
+"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022\n"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_PT\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
+"Language: tr_TR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Não foi possível carregar esta secção."
+msgstr "Bu bölüm yüklenemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr "Não foi possível carregar o formulário de avaliação da Equipa."
+msgstr "Personel değerlendirme formu yüklenemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
-msgstr "Não foi possível carregar a exibição de respostas entregues não classificadas."
+msgstr "Notlandırılmamış ve kontrol edilmemiş cevapların görüntülenmesi yüklenemez."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Não foi possível submeter esta resposta."
+msgstr "Bu cevap gönderilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Não foi possível guardar esta resposta."
+msgstr "Bu cevap kaydedilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Não foi possível submeter este comentário."
+msgstr "Bu geri bildirim gönderilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Não foi possível submeter esta avaliação."
+msgstr "Bu değerlendirme gönderilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Ocorreu erro no reagendamento de uma ou mais tarefas."
+msgstr "Bir veya daha fazla yeniden zamanlama görevi başarısız oldu."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Não foi possível gravar este problema."
+msgstr "Bu problem kaydedilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Não foi possível contactar o servidor."
+msgstr "Sunucu ile bağlantı kurulamadı."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Não foi possível recuperar o url de envio."
+msgstr "Yükleme URL'ine erişilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr "Erro de servidor."
+msgstr "Sunucu hatası."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "Não foi possível obter os dados a partir do URL definido."
+msgstr "İndirme bağlantısına erişilemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr "Não foi possível remover a submissão da pool de classificação."
+msgstr "Yükleme not havuzundan kaldırılamadı."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
-msgstr "Várias equipas voltaram para o curso"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:677
 msgid "Could not load teams information."
-msgstr "Não foi possível carregar informação das equipas."
+msgstr "Takım bilgileri yüklenemedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:699
 msgid "User lookup failed"
-msgstr "A procura do utilizador falhou"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:704
 msgid "Error when looking up username"
-msgstr "Erro ao procurar o nome de utilizador"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:728
 msgid "Failed to clone rubric"
-msgstr "Falha na clonagem da rubrica"
+msgstr "Dereceli puanlama anahtarı klonlanamadı"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "View and grade responses"
-msgstr "Ver e classificar as respostas"
+msgstr "Cevapları görüntüle ve notlandır"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
-msgstr "Demonstração da nova experiência de classificação"
+msgstr "Yeni Notlandırma Deneyimi demosu"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
-msgstr "Título da Unidade"
+msgstr "Ünite İsmi"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr "Unidades"
+msgstr "Üniteler"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
-msgstr "Avaliação"
+msgstr "Değerlendirme"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:106
 msgid "Assessments"
-msgstr "Avaliações"
+msgstr "Değerlendirmeler"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:113
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:114
 msgid "Total Responses"
-msgstr "Total de Respostas"
+msgstr "Toplam Cevaplar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:121
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:122
 msgid "Training"
-msgstr "Formação"
+msgstr "Alıştırma"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:129
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:130
 msgid "Peer"
-msgstr "Par"
+msgstr "Kişi"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:137
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:138
 msgid "Self"
-msgstr "Auto"
+msgstr "Kendin"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:145
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:146
 msgid "Waiting"
-msgstr "A aguardar"
+msgstr "Bekleniyor"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr "Equipa"
+msgstr "Personel"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
-msgstr "Nota Final Recebida"
+msgstr "Final Notu Alındı"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
-msgstr "Graduador de Pessoal"
+msgstr "Personel Notlandırması"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
-msgstr "Lista de Avaliações Abertas não está disponível"
+msgstr "Açık Değerlendirmeler Listesi mevcut değil"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr "Aguarde, por favor"
+msgstr "Lütfen bekleyin"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
-msgstr "A visualização em grelha não está disponível"
+msgstr "Blok görünüm mevcut değil"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
-msgstr "Voltar à lista completa"
+msgstr "Tam Listeye Dön"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
-msgstr "Confirmar"
+msgstr "Onayla"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:7
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "İptal"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
-msgstr "O seu ficheiro foi eliminado ou o caminho foi alterado: "
+msgstr "Dosyanız silindi veya kayıt yeri değiştirildi: "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Estado da sua Resposta"
+msgstr "Cevabınızın Durumu"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Esta resposta não foi guardada."
+msgstr "Bu cevap kaydedilmedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
-msgstr "Caso saia desta página sem gravar ou submeter a sua resposta, irá perder todo o trabalho até aqui realizado."
+msgstr "Eğer sayfadan cevabınızı kaydetmeden ya da göndermeden ayrılırsanız, cevap için yaptığınız işlemleri kaybedeceksiniz."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "A guardar..."
+msgstr "Kaydediliyor..."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Esta resposta foi guardada mas não foi submetida."
+msgstr "Bu cevap kaydedildi, ancak gönderilmedi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Erro"
+msgstr "Hata"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
-msgstr "Confirmar Submissão da Resposta"
+msgstr "Yanıt Gönderimini Doğrula"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr "Está prestes a submeter a sua resposta para esta tarefa. Depois de a submeter, não é possível alterá-la ou submeter uma nova resposta."
+msgstr "Bu görev için cevabını göndermek üzeresin. Cevabını gönderdikten sonra, cevabı değiştiremez veya yeni bir cevap ekleyemezsin."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
-msgstr "O tamanho do ficheiro individual deve ser {max_files_mb}MB ou menos."
+msgstr "Her bir dosyanın boyutu {max_files_mb}MB ya da daha az olmalı."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:590
 msgid ""
 "File upload failed: unsupported file type. Only the supported file types can"
 " be uploaded. If you have questions, please reach out to the course team."
-msgstr "Falha no carregamento do ficheiro: tipo de ficheiro não suportado. Apenas os tipos de ficheiros suportados podem ser carregados. Se tiver dúvidas, entre em contato com a equipa de curso."
+msgstr "Dosya yükleme başarısız oldu: desteklenmeyen dosya türü. Yalnızca desteklenen dosya türleri yüklenebilir. Sorularınız varsa lütfen ders ekibiyle iletişime geçin."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
-msgstr "O número máximo de ficheiros que podem ser guardados é "
+msgstr "Kaydedilebilecek maksimum dosya sayısı "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 #: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
-msgstr "Descreva "
+msgstr "Tanımla"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 msgid "(required):"
-msgstr "(obrigatório):"
+msgstr "(gerekli):"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
-msgstr "Visualização em miniatura de "
+msgstr "Küçük resim"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
-msgstr "Confirmar exclusão do arquivo enviado"
+msgstr "Yüklenmiş Dosyayı Silmeyi Onaylayın"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:805
 msgid ""
 "Are you sure you want to delete the following file? It cannot be restored.\n"
 "File: "
-msgstr "Tem certeza de que deseja apagar o seguinte ficheiro? Não pode ser restaurado.\nFicheiro: "
+msgstr "Bu dosyayı silmek istediğinize emin misiniz? Bu işlem geri alınamaz.\nDosya: "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_self.js:138
 msgid ""
 "If you leave this page without submitting your self assessment, you will "
 "lose any work you have done."
-msgstr "Caso saia desta página sem submeter a sua auto-avaliação, irá perder todo o trabalho até aqui realizado."
+msgstr "Bu sayfayı değerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:143
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:253
 msgid "Unexpected server error."
-msgstr "Erro do servidor."
+msgstr "Beklenmeyen sunucu hatası."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:147
 msgid "You must provide a learner name."
-msgstr "Deve indicar o nome de um estudante."
+msgstr "Bir öğrenci ismi belirtmelisiniz."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:214
 msgid ""
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
-msgstr "Esta nota será aplicada a todos os membros da equipa. Quer continuar?"
+msgstr "Bu not takımın tüm üyelerine uygulanacak. Devam etmek istiyor musunuz?"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
-msgstr "Confirme o envio da equipe de notas"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
-msgstr "Erro ao obter o número de respostas sem classificação"
+msgstr "Notlandırılmamış cevapların sayısını çekmede hata"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:538
 msgid ""
 "If you leave this page without submitting your staff assessment, you will "
 "lose any work you have done."
-msgstr "Caso saia desta página sem submeter a sua avaliação individual, irá perder todo o trabalho até aqui realizado."
+msgstr "Bu sayfayı ekip değerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_training.js:130
 msgid "Feedback available for selection."
-msgstr "Comentário disponível para a seleção."
+msgstr "Seçilenler için geri bildirim mümkün."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_peer.js:217
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
-msgstr "Caso saia desta página sem submeter o seu teste, irá perder todo o trabalho até aqui realizado."
+msgstr "Bu sayfayı özdeğerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
-msgstr "Atualizar"
+msgstr "Yenile"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
-msgstr "Nome de utilizador"
+msgstr "Kullanıcı adı"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peers Assessed"
-msgstr "Colegas avaliados"
+msgstr "Akran Değerlendirmesi"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peer Responses Received"
-msgstr "Respostas de Colegas Recebidas"
+msgstr "Akran Cevapları Alındı"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Time Spent On Current Step"
-msgstr "Tempo Gasto Na Etapa Atual"
+msgstr "Mevcut Adımda Harcanan Zaman"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Staff assessment"
-msgstr "Avaliação da equipa"
+msgstr "Personel değerlendirmesi"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Grade Status"
-msgstr "Estado da Classificação"
+msgstr "Not Durumu"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "The \"{name}\" problem is configured to require a minimum of {min_grades} "
 "peer grades, and asks to review {min_graded} peers."
-msgstr "O problema \"{name}\" está configurado para exigir um mínimo de {min_grades} avaliações de colegas, e pede para rever {min_graded} colegas."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "There are currently {stuck_learners} learners in the waiting state, meaning "
 "they have not yet met all requirements for Peer Assessment. "
-msgstr "Existem atualmente {stuck_learners} estudantes no estado de espera, o que significa que ainda não cumpriram todos os requisitos para a Avaliação por Colegas. "
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "However, {overwritten_count} of these students have received a grade through"
 " the staff grade override tool already."
-msgstr "No entanto, {overwritten_count} destes estudantes já receberam uma classificação através da ferramenta de substituição de classificações da equipa."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
-msgstr "Erro ao ir buscar dados de estudantes."
+msgstr "Öğrenci verisi alınırken hata oluştu."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
-msgstr "Não foi possível carregar"
+msgstr "Yüklenemedi"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Parágrafo"
+msgstr "Paragraf"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Pré-formatado"
+msgstr "Önceden biçimlendirilmiş"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Título 3"
+msgstr "Başlık 3"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Título 4"
+msgstr "Başlık 4"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Título 5"
+msgstr "Başlık 5"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Título 6"
+msgstr "Başlık 6"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Opção sem título"
+msgstr "Adlandırılmamış Seçenek"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Não Selecionado"
+msgstr "Seçilmedi"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
-msgstr "Rúbrica de clonagem de problemas"
+msgstr "Dereceli puanlama anahtarını klonlamada problem"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr "Critério Adicionado"
+msgstr "Ölçüt Eklendi"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
-msgstr "Adicionou um critério. Terá de selecionar uma opção para o critério na etapa de Formação do Estudante. Para o fazer, clique no separador Passos de Avaliação."
+msgstr "Bir ölçüt eklediniz. Öğrenci Eğitimi adımında, ölçüt için bir seçenek belirlemelisiniz. Bunu yapmak için, Değerlendirme Adımları sekmesine tıklayınız."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Opção eliminada"
+msgstr "Seçenek Silindi"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr "Eliminou uma opção. Esta opção foi removida do seu critério nos exemplos de respostas da etapa Formação do Estudante. Deve selecionar uma nova opção para esse critério."
+msgstr "Bir seçenek sildiniz. Sistem, Öğrenci Eğitimi adımında yer alan örnek cevaplardaki ölçütten bu seçenek kaldırıldı. Bu ölçüt için yeni bir seçenek seçmeniz gerekebilir."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr "Eliminou todas as opções para este critério. O critério foi removido dos exemplos de resposta da etapa de Formação do Estudante."
+msgstr "Bu ölçüt için tüm seçenekleri sildiniz. Öğrenci Eğitimi adımındaki örnek cevaplardan ölçüt kaldırıldı."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr "Critério eliminado"
+msgstr "Ölçüt Silindi"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr "Eliminou um critério. O critério foi removido dos exemplos de resposta da etapa de Formação do Estudante."
+msgstr "Bir ölçüt sildiniz. Sistem, Öğrenci Eğitimi adımındaki örnek cevaplardan ölçüt kaldırıldı."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Aviso"
+msgstr "Uyarı"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr "As alterações às etapas que não estão selecionados como parte da tarefa, não serão guardadas."
+msgstr "Görevin bir parçası olarak seçili olmayan adımlardaki değişiklikler kaydedilmeyecek."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr "O tipo de ficheiro não pode estar vazio."
+msgstr "Dosya türü boş olamaz."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr "Os seguintes tipos de ficheiro não são permitidos: "
+msgstr "Aşağıdaki dosya türüne izin  verilmiyor:"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
-msgstr "Sem Sucesso ao Guardar"
+msgstr "Kaydetme Başarısız"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
-msgstr "Erros detetados nos seguintes separadores: "
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 msgid ""
 "This ORA has already been released. Changes will only affect learners making"
 " new submissions. Existing submissions will not be modified by this change."
-msgstr "Esta Questão de Resposta Aberta já foi divulgada. As alterações apenas irão afetar os alunos que fizerem novas submissões. As submissões existentes não serão modificadas por esta alteração."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:318
 msgid "error count: "
-msgstr "contagem de erros: "
+msgstr ""
```

### Comparing `ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Bogdan Mateescu, 2018
-# Pinman <bogdan.stefan@outlook.com>, 2014
-# Rares Mihai Popa <raresmihaipopa@gmail.com>, 2015
-# tyby94 <tyby04@gmail.com>, 2014
+# Faton Nuha <faton11@live.com>, 2014-2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Bogdan Mateescu, 2018\n"
-"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
+"Last-Translator: Faton Nuha <faton11@live.com>, 2014-2016\n"
+"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/language/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: sq\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
@@ -43,20 +40,20 @@
 "Example {example_number} has an invalid option for \"{criterion_name}\": "
 "\"{option_name}\""
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:227
 #, python-brace-format
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
-msgstr ""
+msgstr "Shempull {example_number} ka një opsion shtesë për \"{criterion_name}\""
 
 #: openassessment/assessment/api/student_training.py:240
 #, python-brace-format
 msgid "Example {example_number} is missing an option for \"{criterion_name}\""
-msgstr ""
+msgstr "Shembull {example_number} është duke munguar një opsion për \"{criterion_name}\""
 
 #: openassessment/data.py:533
 #, python-brace-format
 msgid "Criterion {number}: {label}"
 msgstr ""
 
 #: openassessment/data.py:535
@@ -145,35 +142,35 @@
 
 #: openassessment/data.py:1320
 msgid "No description provided."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:28
 msgid "Save"
-msgstr "Salvează"
+msgstr "Ruaj"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
-msgstr "Anulează"
+msgstr "Anulo"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:5
 msgid "Display Name "
-msgstr "Nume afisat"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:8
 msgid "The display name for this component."
-msgstr "Numele afișat pentru acest element."
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:12
 msgid "Text Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:20
 msgid ""
@@ -215,15 +212,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:53
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:94
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:132
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:158
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:46
 msgid "True"
-msgstr "Adevarat"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:56
 msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
@@ -327,48 +324,48 @@
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:9
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:7
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:10
 msgid "Remove"
-msgstr "Inlatura"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:17
 msgid "Criterion Name"
-msgstr ""
+msgstr "Emri i kriterit"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:29
 msgid "Criterion Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:44
 msgid "Add Option"
-msgstr ""
+msgstr "Shto një opsion"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:52
 msgid "Feedback for This Criterion"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:54
 #: openassessment/xblock/studio_mixin.py:49
 msgid "None"
-msgstr "Nimic"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:55
 #: openassessment/xblock/studio_mixin.py:48
 msgid "Optional"
-msgstr ""
+msgstr "Opcionale"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:56
 #: openassessment/templates/openassessmentblock/oa_rubric.html:13
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:93
 #: openassessment/xblock/studio_mixin.py:47
 msgid "Required"
-msgstr "Necesar"
+msgstr "E detyrueshme"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:61
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
@@ -379,27 +376,27 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:8
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:7
 msgid "Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:15
 msgid "Rubric"
-msgstr "Rubrica"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:22
 msgid "Schedule"
-msgstr "Program"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr "Setări"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
@@ -468,30 +465,30 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:5
 msgid "Peer Assessment Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:10
 msgid "Start Date"
-msgstr "Data de început"
+msgstr "Data e fillimit"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:19
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:19
 msgid "Start Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:119
 msgid "Due Date"
-msgstr "Data Scadentă"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:40
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:40
 msgid "Due Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:48
@@ -629,15 +626,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:22
 msgid "View / Add Sample Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:32
 msgid "Add Sample Response"
-msgstr ""
+msgstr "Shto një përgjigjje të thjeshtë"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:4
 msgid "Clone Rubric"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:7
 msgid ""
@@ -673,25 +670,25 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr "Răspuns:"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
-msgstr "Nu a fost Selectat"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:128
 msgid "points"
-msgstr "puncte"
+msgstr "pikët"
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
@@ -703,31 +700,30 @@
 "\n"
 "                      %(assessment_title)s - %(points)s point\n"
 "                  "
 msgid_plural ""
 "\n"
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
-msgstr[0] "\n                      %(assessment_title)s - %(points)s punct\n                  "
-msgstr[1] "\n                      %(assessment_title)s - %(points)s puncte\n                  "
-msgstr[2] "\n                      %(assessment_title)s - %(points)s de puncte\n                  "
+msgstr[0] ""
+msgstr[1] ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:24
 #, python-format
 msgid "More information about %(name)s"
-msgstr ""
+msgstr "Më shumë informacione rreth %(name)s"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
 msgid "Your Grade"
-msgstr "Nota dvs."
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:19
 #, python-format
 msgid ""
 "\n"
 "                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
@@ -744,15 +740,15 @@
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr ""
+msgstr "Përgjigjja juaj"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
@@ -774,24 +770,24 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:31
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:29
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:25
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:30
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:27
 msgid "Status"
-msgstr "Status"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:65
 msgid "Overall Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:70
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:28
 msgid "Points"
-msgstr ""
+msgstr "Pikët"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:96
 msgid "Additional comments on your response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:117
 msgid "Provide feedback on peer assessments"
@@ -850,19 +846,19 @@
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr ""
+msgstr "E pa kompletuar"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
-msgstr ""
+msgstr "Ju nuk keni kompletuar të gjitha hapat e këtij problemi."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:27
 msgid "You have not started this problem yet."
@@ -891,30 +887,30 @@
 msgid ""
 "Grade Available Responses is unavailable. This item is not configured for "
 "Staff Assessment."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html:6
 msgid "Please wait"
-msgstr "Vă rugăm așteptați"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:15
 msgid "Waiting Step Details"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:24
 msgid ""
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:20
 #, python-format
 msgid "%(num_points)s points"
-msgstr ""
+msgstr "%(num_points)s pikë"
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:24
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:74
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:53
 msgid "Your peer's response to the prompt above"
 msgstr ""
 
@@ -1071,15 +1067,15 @@
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
-msgstr "Se încarcă"
+msgstr "Duke u ngarkuar"
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
 msgid "Preview in LaTeX"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:10
 msgid "Click to preview your submission in LaTeX."
@@ -1087,15 +1083,15 @@
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:15
 msgid "Preview Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
-msgstr "Comentarii"
+msgstr "Komentet"
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
@@ -1179,15 +1175,15 @@
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html:19
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:21
 #: openassessment/templates/openassessmentblock/self/oa_self_cancelled.html:21
 #: openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html:18
 #: openassessment/xblock/staff_assessment_mixin.py:172
 msgid "Cancelled"
-msgstr "Anulat"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html:20
 #, python-format
 msgid ""
 "\n"
 "            Incomplete (%(num_graded)s of %(num_must_grade)s)\n"
 "        "
@@ -1198,15 +1194,15 @@
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr "Completat"
+msgstr "Kompletuar"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
@@ -1286,15 +1282,15 @@
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
-msgstr "În Progres"
+msgstr "Në progres"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
@@ -1329,15 +1325,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:104
 msgid ""
 "You can save your progress and return to complete your response at any time."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:106
 msgid "After you submit your response, you cannot edit it"
-msgstr ""
+msgstr "Pasi të e paraqisni përgjgijjen tuaj, ju nuk mund të e ndryshosh atë"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:116
 msgid "What will this assignment be graded on?"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:130
 msgid "The prompt for this section"
@@ -1373,15 +1369,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:244
 msgid "(Required)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:175
 #: openassessment/templates/openassessmentblock/response/oa_response.html:246
 msgid "(Optional)"
-msgstr "(Optional)"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:179
 msgid ""
 "\n"
 "                                              Teams should designate one team member to submit a response on behalf of the\n"
 "                                              entire team.  All team members can use this space to work on draft responses,\n"
 "                                              but you will not be able to see your teammates' drafts made in this space, so\n"
@@ -1492,19 +1488,19 @@
 "\n"
 "                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
-msgstr ""
+msgstr "Ne nuk po mundemi të e paraqesim përgjigjjen tuaj"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:334
 msgid "Submit your response and move to the next step"
-msgstr ""
+msgstr "Paraqiteni përgjigjjen tuaj dhe kaloni në hapin tjetër"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:34
 msgid "Your submission was cancelled. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:37
 #, python-format
@@ -1530,15 +1526,15 @@
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:19
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:20
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
-msgstr "Incomplet"
+msgstr "E pa kompletuar"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
@@ -1547,15 +1543,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:20
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:20
 #: openassessment/templates/openassessmentblock/self/oa_self_complete.html:18
 #: openassessment/templates/openassessmentblock/student_training/student_training_complete.html:17
 #: openassessment/xblock/staff_assessment_mixin.py:179
 #: openassessment/xblock/staff_assessment_mixin.py:202
 msgid "Complete"
-msgstr "Complet"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:51
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:57
 msgid "Your response"
 msgstr ""
 
@@ -1592,15 +1588,15 @@
 "\n"
 "                        You still need to complete the %(start_tag)sself assessment%(end_tag)s step.\n"
 "                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:15
 msgid "Error"
-msgstr "Eroare"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:29
 #, python-format
 msgid ""
 "\n"
 "                            You joined Team %(team_name)s after they submitted a response for this assignment\n"
 "                            and you will not receive a grade for their response. You have also not previously submitted\n"
@@ -1673,15 +1669,15 @@
 msgid "View ORA in Studio"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:69
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:151
 msgid "Close"
-msgstr "Închide"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:37
 msgid "Manage Teams"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:50
 msgid "Enter an individual learner's username or email"
@@ -1689,23 +1685,23 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:52
 msgid "Enter a team member's username or edX email"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:56
 msgid "Submit"
-msgstr "Trimite"
+msgstr "Paraqit"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:78
 msgid "Response total"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:84
 msgid "Location"
-msgstr "Locație"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:90
 msgid "Learner Progress"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:94
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:117
@@ -1723,15 +1719,15 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:118
 msgid "Release Date"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:131
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:137
 msgid "N/A"
-msgstr "N/A"
+msgstr "N/A "
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
@@ -1772,15 +1768,15 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:57
 msgid "The learner's response to the prompt above"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:64
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:57
 msgid "Submit assessment"
-msgstr "Trimite evaluarea"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:70
 msgid "Submit assessment and continue grading"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html:6
 #, python-format
@@ -1903,15 +1899,14 @@
 "                                    "
 msgid_plural ""
 "\n"
 "                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:165
 msgid "The submission is waiting for assessments."
@@ -2018,15 +2013,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
-msgstr ""
+msgstr "Pikët e mundshme"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:27
 #, python-format
@@ -2284,15 +2279,15 @@
 msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:52
 #, python-brace-format
 msgid ""
 "'{date}' is an invalid date format. Make sure the date is formatted as YYYY-"
 "MM-DDTHH:MM:SS."
-msgstr ""
+msgstr "'{date}' është një datë jo valide. Sigurohuni që formati i datës është VVVV-MM-DDTHH:MM:SS"
 
 #: openassessment/xblock/resolve_dates.py:57
 #, python-brace-format
 msgid "'{date}' must be a date string or datetime"
 msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:210
@@ -2528,15 +2523,15 @@
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:261
 msgid "This response could not be saved."
-msgstr "Acest raspuns nu poate fi salvat."
+msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:265
 msgid "This response was not submitted."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:281
 msgid "Files descriptions were not submitted."
@@ -2562,19 +2557,19 @@
 
 #: openassessment/xblock/submission_mixin.py:508
 msgid "Error retrieving upload URL."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:790
 msgid "This response has been saved but not submitted."
-msgstr "Acest răspuns a fost salvat dar nu trimis."
+msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:791
 msgid "This response has not been saved."
-msgstr "Răspunsul nu a fost salvat."
+msgstr ""
 
 #: openassessment/xblock/validation.py:118
 msgid "This problem must include at least one assessment."
 msgstr ""
 
 #: openassessment/xblock/validation.py:122
 msgid "The assessment order you selected is invalid."
```

### Comparing `ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ro/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,119 +1,116 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Alexandra <elenadintroia1986@yahoo.com>, 2015
-# Alex Coman <itsalexcoman@gmail.com>, 2019
-# Irina Maria Curuia, 2015
-# Manuel, 2021
+# Vladimír Záhradník <vladimir@zahradnik.io>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Manuel, 2021\n"
-"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
+"Last-Translator: Vladimír Záhradník <vladimir@zahradnik.io>, 2015\n"
+"Language-Team: Slovak (http://app.transifex.com/open-edx/edx-platform/language/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: sk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Această secţiune nu a putut fi încărcată."
+msgstr "Túto sekciu nie je možné načítať."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr "Formularul de evaluare a personalului nu a putut fi încărcat."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Acest răspuns nu a putut fi trimis."
+msgstr "Túto odpoveď nie je možné odoslať."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Acest răspuns nu a putut fi salvat."
+msgstr "Túto odpoveď nie je možné uložiť."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Feedback-ul nu a putut fi trimis."
+msgstr "Túto spätnú väzbu nie je možné odoslať."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Această evaluare nu a putut fi trimisă."
+msgstr "Toto hodnotenie nie je možné odoslať."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Una sau mai multe reprogramări au eşuat."
+msgstr "Jedna alebo viac úloh pre zmenu termínu zlyhala."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Această problemă nu a putut fi salvată."
+msgstr "Túto úlohu nebolo možné uložiť."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Serverul nu a putut fi contactat."
+msgstr "Nebolo možné kontaktovať server."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Nu s-a putut obţine linkul de încărcare."
+msgstr "Nebolo možné získať url adresu pre odovzdanie obsahu."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr "Eroare de server."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "Nu s-a putut obţine linkul de descărcare."
+msgstr "Nebolo možné získať adresu pre prevzatie obsahu."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr ""
+msgstr "Toto podanie nebolo možné odstrániť z klasifikačného hárku."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
 msgstr ""
 
@@ -253,54 +250,54 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Statusul răspunsului tău"
+msgstr "Stav vašej odpovede"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Acest răspuns nu a fost salvat."
+msgstr "Odpoveď nebola uložená."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Se salvează..."
+msgstr "Ukladá sa..."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Acest răspuns a fost salvat, dar nu și trimis."
+msgstr "Táto odpoveď bola uložená, ale nebola odoslaná."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Eroare"
+msgstr "Chyba"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr ""
+msgstr "Chystáte sa odoslať vašu odpoveď pre toto zadanie. Potom ako túto odpoveď odošlete, nebudete ju môcť zmeniť ani nebudete môcť odoslať novú odpoveď."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -451,123 +448,123 @@
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Paragraf"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Preformatat"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Titlu 3"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Titlu 4"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Titlu 5"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Titlu 6"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr ""
+msgstr "Nepomenovaná voľba"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr ""
+msgstr "Nie je vybrané"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr ""
+msgstr "Pridané kritérium"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr ""
+msgstr "Voľba odstránená"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr ""
+msgstr "Odstránili ste voľbu. Táto voľba bola vymazaná z pridruženého kritéria vo vzorových odpovediach v koku Výcvik študentov. Pravdepodobne budete musieť pre toto kritérium zvoliť novú voľbu."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr ""
+msgstr "Odstránili ste všetky voľby pre toto kritérium. Toto kritérium bolo vymazané zo všetkých vzorových odpovedí v kroku Výcvik študentov."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr ""
+msgstr "Kritérium odstránené"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr ""
+msgstr "Odstránili ste kritérium. Toto kritérium bolo vymazané zo všetkých vzorových odpovedí v kroku Výcvik študentov."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr ""
+msgstr "Upozornenie"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr ""
+msgstr "Zmeny pre kroky, ktoré nie sú zvolené ako súčasť tohto zadania, nebudú uložené."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr ""
+msgstr "Typy súborov nemôžu byť prázdne."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr ""
+msgstr "Nasledujúce typy súborov nie sú povolené:"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
```

### Comparing `ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/ru/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sk/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sk/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Vladimír Záhradník <vladimir@zahradnik.io>, 2015
+# 7b361a451bd8feeed2dbd9245f836232_a786ad5 <aefa5f09660e622131eca858f9656914_301034>, 2015
+# Hoà Lê Thanh <hoa.lethanh@gmail.com>, 2017
+# NGUYEN CONG NAM <congnam0409@gmail.com>, 2014
+# Nguyen Don Binh <donbinhvn@gmail.com>, 2014
+# NGUYEN HOANG AN <neyugn2909@gmail.com>, 2014
+# Nguyen Nhat Quang <technicalmanager@gmail.com>, 2016
+# Theodora. Tôn Nữ Quý Thiện <thien.tonnu1001@gmail.com>, 2015
+# Le Minh Tri <trilm@hihexa.com>, 2020
+# Trung V. Nguyen <trung.ngvan@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Vladimír Záhradník <vladimir@zahradnik.io>, 2015\n"
-"Language-Team: Slovak (http://app.transifex.com/open-edx/edx-platform/language/sk/)\n"
+"Last-Translator: Le Minh Tri <trilm@hihexa.com>, 2020\n"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: vi\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Túto sekciu nie je možné načítať."
+msgstr "Không thể tải mục này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
 msgstr ""
 
@@ -39,78 +47,78 @@
 msgid "The display of ungraded and checked out responses could not be loaded."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Túto odpoveď nie je možné odoslať."
+msgstr "Không thể gửi câu trả lời này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Túto odpoveď nie je možné uložiť."
+msgstr "Không thể lưu câu trả lời này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Túto spätnú väzbu nie je možné odoslať."
+msgstr "Không thể gửi phản hồi này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Toto hodnotenie nie je možné odoslať."
+msgstr "Không thể gửi đánh giá này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Jedna alebo viac úloh pre zmenu termínu zlyhala."
+msgstr "Một hoặc nhiều tác vụ điều chỉnh lịch học đã thất bại."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Túto úlohu nebolo možné uložiť."
+msgstr "Không thể lưu câu hỏi này."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Nebolo možné kontaktovať server."
+msgstr "Không thể liên hệ với máy chủ."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Nebolo možné získať url adresu pre odovzdanie obsahu."
+msgstr "Không thể tìm thấy đường dẫn tải lên."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "Nebolo možné získať adresu pre prevzatie obsahu."
+msgstr "Không thể tìm thấy đường dẫn tải xuống."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr "Toto podanie nebolo možné odstrániť z klasifikačného hárku."
+msgstr "Bài nộp không thể gỡ bỏ khỏi hệ thống chấm điểm."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
 msgstr ""
 
@@ -250,54 +258,54 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Stav vašej odpovede"
+msgstr "Trạng Thái Trả Lời Của Bạn"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Odpoveď nebola uložená."
+msgstr "Câu trả lời này chưa được lưu."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Ukladá sa..."
+msgstr "Đang lưu..."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Táto odpoveď bola uložená, ale nebola odoslaná."
+msgstr "Câu trả lời này đã được lưu nhưng chưa được gửi đi."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Chyba"
+msgstr "Lỗi"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr "Chystáte sa odoslať vašu odpoveď pre toto zadanie. Potom ako túto odpoveď odošlete, nebudete ju môcť zmeniť ani nebudete môcť odoslať novú odpoveď."
+msgstr "Bạn sắp nộp câu trả lời cho bài tập này. Sau khi gửi bài bạn sẽ không thể chỉnh sửa hoặc nộp bài mới. "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -478,93 +486,93 @@
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Nepomenovaná voľba"
+msgstr "Tùy Chọn Chưa Đặt Tên"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Nie je vybrané"
+msgstr "Không Được Chọn"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr "Pridané kritérium"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Voľba odstránená"
+msgstr "Đã Xóa Tùy Chọn"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr "Odstránili ste voľbu. Táto voľba bola vymazaná z pridruženého kritéria vo vzorových odpovediach v koku Výcvik študentov. Pravdepodobne budete musieť pre toto kritérium zvoliť novú voľbu."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr "Odstránili ste všetky voľby pre toto kritérium. Toto kritérium bolo vymazané zo všetkých vzorových odpovedí v kroku Výcvik študentov."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr "Kritérium odstránené"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr "Odstránili ste kritérium. Toto kritérium bolo vymazané zo všetkých vzorových odpovedí v kroku Výcvik študentov."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Upozornenie"
+msgstr "Cảnh báo"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr "Zmeny pre kroky, ktoré nie sú zvolené ako súčasť tohto zadania, nebudú uložené."
+msgstr "Những thay đổi ở các bước không được chọn thuộc một phần của bài tập sẽ không được lưu."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr "Typy súborov nemôžu byť prázdne."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr "Nasledujúce typy súborov nie sú povolené:"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
```

### Comparing `ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Faton Nuha <faton11@live.com>, 2014-2016
+# Alina Kozoriz <alinakozoriz@gmail.com>, 2015
+# Andrey Kryachko, 2018
+# Andrii Parkhomenko <andriy.parhomenko@gmail.com>, 2017-2018,2020
+# Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021
+# Dmytro Halko <dgalko@edpro.com.ua>, 2018
+# Irene Korotkova <irca.gav@gmail.com>, 2017
+# Natalia Vynogradenko <tannaha@gmail.com>, 2017-2018
+# fayçal fatihi <ofaycal.geo.x@gmail.com>, 2014
+# olexiim <olexiim@gmail.com>, 2016
+# Olga Filipova <chudaol@gmail.com>, 2015,2017
+# Radmila Segol <geroneja@yahoo.com>, 2017
+# Tanya Korshun, 2014
+# Zoriana Zaiats, 2015
+# Юлия, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Faton Nuha <faton11@live.com>, 2014-2016\n"
-"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/language/sq/)\n"
+"Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
+"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/language/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sq\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
-msgstr ""
+msgstr "Не вдалося проаналізувати серіалізовану рубрику"
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
 "If your assignment includes a learner training step, the rubric must have at"
 " least one criterion, and that criterion must have at least one option."
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:203
 #, python-brace-format
 msgid "Example {example_number} has a validation error: {error}"
-msgstr ""
+msgstr "Приклад {example_number} має помилку перевірки: {error} "
 
 #: openassessment/assessment/api/student_training.py:217
 #, python-brace-format
 msgid ""
 "Example {example_number} has an invalid option for \"{criterion_name}\": "
 "\"{option_name}\""
-msgstr ""
+msgstr "Приклад {example_number} має недійсний параметр для \"{criterion_name}\": \"{option_name}\""
 
 #: openassessment/assessment/api/student_training.py:227
 #, python-brace-format
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
-msgstr "Shempull {example_number} ka një opsion shtesë për \"{criterion_name}\""
+msgstr ""
 
 #: openassessment/assessment/api/student_training.py:240
 #, python-brace-format
 msgid "Example {example_number} is missing an option for \"{criterion_name}\""
-msgstr "Shembull {example_number} është duke munguar një opsion për \"{criterion_name}\""
+msgstr ""
 
 #: openassessment/data.py:533
 #, python-brace-format
 msgid "Criterion {number}: {label}"
 msgstr ""
 
 #: openassessment/data.py:535
@@ -142,19 +155,19 @@
 
 #: openassessment/data.py:1320
 msgid "No description provided."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:28
 msgid "Save"
-msgstr "Ruaj"
+msgstr "Зберегти"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
-msgstr "Anulo"
+msgstr "Відмінити"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
@@ -227,15 +240,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:58
 msgid "File Upload Types"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:60
 msgid "PDF or Image Files"
-msgstr ""
+msgstr "PDF або файл зображення"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:61
 msgid "Image Files"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:62
 msgid "Custom File Types"
@@ -328,44 +341,44 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:10
 msgid "Remove"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:17
 msgid "Criterion Name"
-msgstr "Emri i kriterit"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:29
 msgid "Criterion Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:44
 msgid "Add Option"
-msgstr "Shto një opsion"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:52
 msgid "Feedback for This Criterion"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:54
 #: openassessment/xblock/studio_mixin.py:49
 msgid "None"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:55
 #: openassessment/xblock/studio_mixin.py:48
 msgid "Optional"
-msgstr "Opcionale"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:56
 #: openassessment/templates/openassessmentblock/oa_rubric.html:13
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:93
 #: openassessment/xblock/studio_mixin.py:47
 msgid "Required"
-msgstr "E detyrueshme"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:61
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
@@ -388,15 +401,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr ""
+msgstr "Налаштування"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
@@ -408,15 +421,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:42
 msgid "Option Explanation"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:10
 msgid "Step: Peer Assessment"
-msgstr ""
+msgstr "Крок: Оцінювання студентами"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:15
 msgid ""
 "Peer Assessment allows students to provide feedback to other students and "
 "also receive feedback from others in their final grade. Often, though not "
 "always, this step is preceded by Self Assessment or Learner Training steps."
 msgstr ""
@@ -465,30 +478,30 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:5
 msgid "Peer Assessment Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:10
 msgid "Start Date"
-msgstr "Data e fillimit"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:19
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:19
 msgid "Start Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:119
 msgid "Due Date"
-msgstr ""
+msgstr "Кінцева дата"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:40
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:40
 msgid "Due Time"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:48
@@ -626,15 +639,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:22
 msgid "View / Add Sample Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:32
 msgid "Add Sample Response"
-msgstr "Shto një përgjigjje të thjeshtë"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:4
 msgid "Clone Rubric"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:7
 msgid ""
@@ -670,25 +683,25 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr ""
+msgstr "Відповідь"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:128
 msgid "points"
-msgstr "pikët"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
@@ -702,19 +715,21 @@
 "                  "
 msgid_plural ""
 "\n"
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:24
 #, python-format
 msgid "More information about %(name)s"
-msgstr "Më shumë informacione rreth %(name)s"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
@@ -740,15 +755,15 @@
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr "Përgjigjja juaj"
+msgstr "Ваша відповідь "
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
@@ -779,15 +794,15 @@
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:65
 msgid "Overall Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:70
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:28
 msgid "Points"
-msgstr "Pikët"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:96
 msgid "Additional comments on your response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:117
 msgid "Provide feedback on peer assessments"
@@ -846,19 +861,19 @@
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr "E pa kompletuar"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
-msgstr "Ju nuk keni kompletuar të gjitha hapat e këtij problemi."
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:27
 msgid "You have not started this problem yet."
@@ -902,15 +917,15 @@
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:20
 #, python-format
 msgid "%(num_points)s points"
-msgstr "%(num_points)s pikë"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:24
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:74
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:53
 msgid "Your peer's response to the prompt above"
 msgstr ""
 
@@ -1067,31 +1082,31 @@
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
-msgstr "Duke u ngarkuar"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
 msgid "Preview in LaTeX"
-msgstr ""
+msgstr "Попередній перегляд у LaTeX"
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:10
 msgid "Click to preview your submission in LaTeX."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:15
 msgid "Preview Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
-msgstr "Komentet"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
@@ -1194,15 +1209,15 @@
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr "Kompletuar"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
@@ -1282,15 +1297,15 @@
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
-msgstr "Në progres"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
@@ -1325,15 +1340,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response.html:104
 msgid ""
 "You can save your progress and return to complete your response at any time."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:106
 msgid "After you submit your response, you cannot edit it"
-msgstr "Pasi të e paraqisni përgjgijjen tuaj, ju nuk mund të e ndryshosh atë"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:116
 msgid "What will this assignment be graded on?"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:130
 msgid "The prompt for this section"
@@ -1488,19 +1503,19 @@
 "\n"
 "                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
-msgstr "Ne nuk po mundemi të e paraqesim përgjigjjen tuaj"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:334
 msgid "Submit your response and move to the next step"
-msgstr "Paraqiteni përgjigjjen tuaj dhe kaloni në hapin tjetër"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:34
 msgid "Your submission was cancelled. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:37
 #, python-format
@@ -1526,15 +1541,15 @@
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:19
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:20
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
-msgstr "E pa kompletuar"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
@@ -1549,15 +1564,15 @@
 msgid "Complete"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:51
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:57
 msgid "Your response"
-msgstr ""
+msgstr "Ваша відповідь"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:33
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:54
 msgid "Your Uploaded Files"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:32
@@ -1685,15 +1700,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:52
 msgid "Enter a team member's username or edX email"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:56
 msgid "Submit"
-msgstr "Paraqit"
+msgstr "Надіслати"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:78
 msgid "Response total"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:84
 msgid "Location"
@@ -1719,15 +1734,15 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:118
 msgid "Release Date"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:131
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:137
 msgid "N/A"
-msgstr "N/A "
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
@@ -1899,14 +1914,16 @@
 "                                    "
 msgid_plural ""
 "\n"
 "                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:165
 msgid "The submission is waiting for assessments."
@@ -2013,15 +2030,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
-msgstr "Pikët e mundshme"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:27
 #, python-format
@@ -2136,15 +2153,15 @@
 #: openassessment/xblock/student_training_mixin.py:56
 #: openassessment/xblock/student_training_mixin.py:264
 msgid "An unexpected error occurred."
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:175
 msgid "Peer Assessment"
-msgstr ""
+msgstr "Оцінювання студентами"
 
 #: openassessment/xblock/grade_mixin.py:177
 msgid "Self Assessment"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:217
 msgid "Assessment feedback could not be saved."
@@ -2279,15 +2296,15 @@
 msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:52
 #, python-brace-format
 msgid ""
 "'{date}' is an invalid date format. Make sure the date is formatted as YYYY-"
 "MM-DDTHH:MM:SS."
-msgstr "'{date}' është një datë jo valide. Sigurohuni që formati i datës është VVVV-MM-DDTHH:MM:SS"
+msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:57
 #, python-brace-format
 msgid "'{date}' must be a date string or datetime"
 msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:210
```

### Comparing `ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sq/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/th/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/th/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,136 +1,138 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Adem Özgür <admozgur@gmail.com>, 2015
-# Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022
-# ali selek <aliselek01@gmail.com>, 2015
-# Emrah Emirtekin <eemirtekin@gmail.com>, 2015
-# Hakan Şenel <hgsenel@gmail.com>, 2017
-# İlker IŞIK <m.ilkerisik@hotmail.com>, 2015-2016
-# Kubilay <kubilayinceoren10@gmail.com>, 2015
-# msare <mervesareakin@gmail.com>, 2014
-# Zeynep Ozdemir <gzeynepozdemir@gmail.com>, 2016
+# LIU,SHU-HAO <jeremy55662004@gmail.com>, 2014
+# JEN-HAO HSIEH <orienthauz@gmail.com>, 2015
+# KUN-MIN SYU <qwer20108@gmail.com>, 2014-2015
+# Lin Yu-Chun <iftwoplustwoequalsfive@gmail.com>, 2014
+# LIU,SHU-HAO <jeremy55662004@gmail.com>, 2015
+# Mose Chen <mosechen@gmail.com>, 2017
+# vincent <orzkng2007@yahoo.com.tw>, 2015
+# Xaver Y.R. Chen <yrchen@atcity.org>, 2014
+# Ya-chi Chang <yacchang@mail.fcu.edu.tw>, 2016
+# Ya-chi Chang <yacchang@mail.fcu.edu.tw>, 2016
+# KUN-MIN SYU <qwer20108@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022\n"
-"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
+"Last-Translator: Mose Chen <mosechen@gmail.com>, 2017\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: tr_TR\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Bu bölüm yüklenemedi."
+msgstr "這個部分無法加載。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr "Personel değerlendirme formu yüklenemedi."
+msgstr "工作人員評分表無法載入。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
-msgstr "Notlandırılmamış ve kontrol edilmemiş cevapların görüntülenmesi yüklenemez."
+msgstr "不分級與已回應的顯示無法載入。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Bu cevap gönderilemedi."
+msgstr "作答無法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Bu cevap kaydedilemedi."
+msgstr "作答無法保存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Bu geri bildirim gönderilemedi."
+msgstr "這條反饋意見無法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Bu değerlendirme gönderilemedi."
+msgstr "這份評分無法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Bir veya daha fazla yeniden zamanlama görevi başarısız oldu."
+msgstr "一個或多個任務重新安排失敗。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Bu problem kaydedilemedi."
+msgstr "此問題無法儲存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Sunucu ile bağlantı kurulamadı."
+msgstr "無法聯繫服務器。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Yükleme URL'ine erişilemedi."
+msgstr "無法找到上傳網址"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr "Sunucu hatası."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "İndirme bağlantısına erişilemedi."
+msgstr "無法找到下載網址"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr "Yükleme not havuzundan kaldırılamadı."
+msgstr "此提交不能從評分庫中移除。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:677
 msgid "Could not load teams information."
-msgstr "Takım bilgileri yüklenemedi."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:699
 msgid "User lookup failed"
 msgstr ""
 
@@ -140,299 +142,299 @@
 msgid "Error when looking up username"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:728
 msgid "Failed to clone rubric"
-msgstr "Dereceli puanlama anahtarı klonlanamadı"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "View and grade responses"
-msgstr "Cevapları görüntüle ve notlandır"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
-msgstr "Yeni Notlandırma Deneyimi demosu"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
-msgstr "Ünite İsmi"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr "Üniteler"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
-msgstr "Değerlendirme"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:106
 msgid "Assessments"
-msgstr "Değerlendirmeler"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:113
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:114
 msgid "Total Responses"
-msgstr "Toplam Cevaplar"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:121
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:122
 msgid "Training"
-msgstr "Alıştırma"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:129
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:130
 msgid "Peer"
-msgstr "Kişi"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:137
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:138
 msgid "Self"
-msgstr "Kendin"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:145
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:146
 msgid "Waiting"
-msgstr "Bekleniyor"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr "Personel"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
-msgstr "Final Notu Alındı"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
-msgstr "Personel Notlandırması"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
-msgstr "Açık Değerlendirmeler Listesi mevcut değil"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr "Lütfen bekleyin"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
-msgstr "Blok görünüm mevcut değil"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
-msgstr "Tam Listeye Dön"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
-msgstr "Onayla"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:7
 msgid "Cancel"
-msgstr "İptal"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
-msgstr "Dosyanız silindi veya kayıt yeri değiştirildi: "
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Cevabınızın Durumu"
+msgstr "您的作答之狀態"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Bu cevap kaydedilmedi."
+msgstr "作答尚未儲存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
-msgstr "Eğer sayfadan cevabınızı kaydetmeden ya da göndermeden ayrılırsanız, cevap için yaptığınız işlemleri kaybedeceksiniz."
+msgstr "如果你沒有儲存或提交你的作答而離開這個頁面，你將遺失你任何已作答的作業。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Kaydediliyor..."
+msgstr "儲存中"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Bu cevap kaydedildi, ancak gönderilmedi."
+msgstr "這一份作答已經儲存了，但仍未提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Hata"
+msgstr "錯誤"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
-msgstr "Yanıt Gönderimini Doğrula"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr "Bu görev için cevabını göndermek üzeresin. Cevabını gönderdikten sonra, cevabı değiştiremez veya yeni bir cevap ekleyemezsin."
+msgstr "您即將送出你的作答，一旦送出作答就不能修改，也無法重新送出新的作答。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
-msgstr "Her bir dosyanın boyutu {max_files_mb}MB ya da daha az olmalı."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:590
 msgid ""
 "File upload failed: unsupported file type. Only the supported file types can"
 " be uploaded. If you have questions, please reach out to the course team."
-msgstr "Dosya yükleme başarısız oldu: desteklenmeyen dosya türü. Yalnızca desteklenen dosya türleri yüklenebilir. Sorularınız varsa lütfen ders ekibiyle iletişime geçin."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
-msgstr "Kaydedilebilecek maksimum dosya sayısı "
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 #: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
-msgstr "Tanımla"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 msgid "(required):"
-msgstr "(gerekli):"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
-msgstr "Küçük resim"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
-msgstr "Yüklenmiş Dosyayı Silmeyi Onaylayın"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:805
 msgid ""
 "Are you sure you want to delete the following file? It cannot be restored.\n"
 "File: "
-msgstr "Bu dosyayı silmek istediğinize emin misiniz? Bu işlem geri alınamaz.\nDosya: "
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_self.js:138
 msgid ""
 "If you leave this page without submitting your self assessment, you will "
 "lose any work you have done."
-msgstr "Bu sayfayı değerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
+msgstr "如果你沒有提交你的自評而離開這個頁面，你將遺失你任何你所做的作業。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:143
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:253
 msgid "Unexpected server error."
-msgstr "Beklenmeyen sunucu hatası."
+msgstr "未預期的伺服器錯誤"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:147
 msgid "You must provide a learner name."
-msgstr "Bir öğrenci ismi belirtmelisiniz."
+msgstr "你必須提供一個學習者全名"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:214
 msgid ""
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
-msgstr "Bu not takımın tüm üyelerine uygulanacak. Devam etmek istiyor musunuz?"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
-msgstr "Notlandırılmamış cevapların sayısını çekmede hata"
+msgstr "錯誤獲取不分級的回應數。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:538
 msgid ""
 "If you leave this page without submitting your staff assessment, you will "
 "lose any work you have done."
-msgstr "Bu sayfayı ekip değerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
+msgstr "如果你沒有提交工作人員評估而離開這個頁面，你將會遺失任何你所做的作業。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_training.js:130
 msgid "Feedback available for selection."
-msgstr "Seçilenler için geri bildirim mümkün."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_peer.js:217
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
-msgstr "Bu sayfayı özdeğerlendirmenizi yazmadan terk etmeniz durumunda, yaptığınız tüm işleri kaybedeceksiniz."
+msgstr "如果你沒有提交同儕互評而離開這個頁面，你將遺失任何這部分的作業。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
-msgstr "Yenile"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
-msgstr "Kullanıcı adı"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peers Assessed"
-msgstr "Akran Değerlendirmesi"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peer Responses Received"
-msgstr "Akran Cevapları Alındı"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Time Spent On Current Step"
-msgstr "Mevcut Adımda Harcanan Zaman"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Staff assessment"
-msgstr "Personel değerlendirmesi"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Grade Status"
-msgstr "Not Durumu"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "The \"{name}\" problem is configured to require a minimum of {min_grades} "
 "peer grades, and asks to review {min_graded} peers."
 msgstr ""
 
@@ -446,138 +448,138 @@
 msgid ""
 "However, {overwritten_count} of these students have received a grade through"
 " the staff grade override tool already."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
-msgstr "Öğrenci verisi alınırken hata oluştu."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
-msgstr "Yüklenemedi"
+msgstr "無法載入"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr "Paragraf"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr "Önceden biçimlendirilmiş"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr "Başlık 3"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr "Başlık 4"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr "Başlık 5"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr "Başlık 6"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Adlandırılmamış Seçenek"
+msgstr "未命名的選項"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Seçilmedi"
+msgstr "未選取"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
-msgstr "Dereceli puanlama anahtarını klonlamada problem"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr "Ölçüt Eklendi"
+msgstr " 增加評分標準"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
-msgstr "Bir ölçüt eklediniz. Öğrenci Eğitimi adımında, ölçüt için bir seçenek belirlemelisiniz. Bunu yapmak için, Değerlendirme Adımları sekmesine tıklayınız."
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Seçenek Silindi"
+msgstr "刪除選項"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr "Bir seçenek sildiniz. Sistem, Öğrenci Eğitimi adımında yer alan örnek cevaplardaki ölçütten bu seçenek kaldırıldı. Bu ölçüt için yeni bir seçenek seçmeniz gerekebilir."
+msgstr "您已經刪除 一個選項。在評分練習步驟中，系統已經從範例作答裡刪除評分標準中的選項。您必須為這評分標準選擇新的選項。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr "Bu ölçüt için tüm seçenekleri sildiniz. Öğrenci Eğitimi adımındaki örnek cevaplardan ölçüt kaldırıldı."
+msgstr "您已經刪除了這評分標準中所有的選項，已經從範例作答裡刪除評分標準。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr "Ölçüt Silindi"
+msgstr "刪除評分標準"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr "Bir ölçüt sildiniz. Sistem, Öğrenci Eğitimi adımındaki örnek cevaplardan ölçüt kaldırıldı."
+msgstr "您已經刪除 一個標準。在評分練習中，該標準已經從範例作答裡刪除。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Uyarı"
+msgstr "警告"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr "Görevin bir parçası olarak seçili olmayan adımlardaki değişiklikler kaydedilmeyecek."
+msgstr "您已取消選擇此評分步驟，這將使它不會被儲存。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr "Dosya türü boş olamaz."
+msgstr "檔案類型不可空白。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr "Aşağıdaki dosya türüne izin  verilmiyor:"
+msgstr "下列檔案類型是不允許的："
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
-msgstr "Kaydetme Başarısız"
+msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
```

### Comparing `ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# Alina Kozoriz <alinakozoriz@gmail.com>, 2015
-# Andrey Kryachko, 2018
-# Andrii Parkhomenko <andriy.parhomenko@gmail.com>, 2017-2018,2020
-# Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021
-# Dmytro Halko <dgalko@edpro.com.ua>, 2018
-# Irene Korotkova <irca.gav@gmail.com>, 2017
-# Natalia Vynogradenko <tannaha@gmail.com>, 2017-2018
-# fayçal fatihi <ofaycal.geo.x@gmail.com>, 2014
-# olexiim <olexiim@gmail.com>, 2016
-# Olga Filipova <chudaol@gmail.com>, 2015,2017
-# Radmila Segol <geroneja@yahoo.com>, 2017
-# Tanya Korshun, 2014
-# Zoriana Zaiats, 2015
-# Юлия, 2015
+# dangitdang <dangpham@mit.edu>, 2014
+# Doan Viet Hung <viethung.doan@gmail.com>, 2014
+# Duong Nguyen <supermanikin@yahoo.com>, 2015
+# Hoà Lê Thanh <hoa.lethanh@gmail.com>, 2017
+# Hoang Ha <halink0803@gmail.com>, 2014
+# hung nguyen <nguyenhungblog@gmail.com>, 2017
+# Le Minh Tri <trilm@hihexa.com>, 2020
+# Lê Như Ý <nhuyle89@gmail.com>, 2014
+# Minh Tue Vo <mvo@edx.org>, 2014
+# NGUYEN CONG NAM <congnam0409@gmail.com>, 2014
+# NGUYEN HOANG AN <neyugn2909@gmail.com>, 2014
+# Lam Nguyen <lamnguyen.cis@gmail.com>, 2020
+# Nguyen Nhat Quang <technicalmanager@gmail.com>, 2016
+# Sarina Canelake <sarina@tcril.org>, 2014
+# Thi Thanh Nga Do <thanhnga.ftu2@gmail.com>, 2015
+# Theodora. Tôn Nữ Quý Thiện <thien.tonnu1001@gmail.com>, 2015
+# Trần Tử Thiêng <trantuthieng26256@gmail.com>, 2014
+# Trung V. Nguyen <trung.ngvan@gmail.com>, 2015
+# Vinh Nguyen <vinhmaivy@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
-"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/language/uk/)\n"
+"Last-Translator: Lam Nguyen <lamnguyen.cis@gmail.com>, 2020\n"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: uk\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Language: vi\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
-msgstr "Не вдалося проаналізувати серіалізовану рубрику"
+msgstr ""
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
 "If your assignment includes a learner training step, the rubric must have at"
 " least one criterion, and that criterion must have at least one option."
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:203
 #, python-brace-format
 msgid "Example {example_number} has a validation error: {error}"
-msgstr "Приклад {example_number} має помилку перевірки: {error} "
+msgstr "Ví dụ {example_number} có một lỗi xác nhận: {error}"
 
 #: openassessment/assessment/api/student_training.py:217
 #, python-brace-format
 msgid ""
 "Example {example_number} has an invalid option for \"{criterion_name}\": "
 "\"{option_name}\""
-msgstr "Приклад {example_number} має недійсний параметр для \"{criterion_name}\": \"{option_name}\""
+msgstr ""
 
 #: openassessment/assessment/api/student_training.py:227
 #, python-brace-format
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
 msgstr ""
 
 #: openassessment/assessment/api/student_training.py:240
@@ -115,15 +120,15 @@
 #: openassessment/data.py:918
 msgid "Anonymous Scorer Id"
 msgstr ""
 
 #: openassessment/data.py:920
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:59
 msgid "Overall Feedback"
-msgstr ""
+msgstr "Phản hồi tổng thể"
 
 #: openassessment/data.py:921
 msgid "Assessment Score Earned"
 msgstr ""
 
 #: openassessment/data.py:922
 msgid "Assessment Scored At"
@@ -155,31 +160,31 @@
 
 #: openassessment/data.py:1320
 msgid "No description provided."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:28
 msgid "Save"
-msgstr "Зберегти"
+msgstr "Lưu"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
-msgstr "Відмінити"
+msgstr "Hủy bỏ"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:5
 msgid "Display Name "
-msgstr ""
+msgstr "Hiểu thị tên"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:8
 msgid "The display name for this component."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:12
 msgid "Text Response"
@@ -217,38 +222,38 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:52
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:93
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:131
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:157
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:45
 msgid "False"
-msgstr ""
+msgstr "Sai"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:53
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:94
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:132
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:158
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:46
 msgid "True"
-msgstr ""
+msgstr "Đúng"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:56
 msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:58
 msgid "File Upload Types"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:60
 msgid "PDF or Image Files"
-msgstr "PDF або файл зображення"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:61
 msgid "Image Files"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:62
 msgid "Custom File Types"
@@ -337,99 +342,99 @@
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:9
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:7
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:10
 msgid "Remove"
-msgstr ""
+msgstr "Loại bỏ"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:17
 msgid "Criterion Name"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:29
 msgid "Criterion Prompt"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:44
 msgid "Add Option"
-msgstr ""
+msgstr "Thêm Tùy chọn"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:52
 msgid "Feedback for This Criterion"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:54
 #: openassessment/xblock/studio_mixin.py:49
 msgid "None"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:55
 #: openassessment/xblock/studio_mixin.py:48
 msgid "Optional"
-msgstr ""
+msgstr "tuỳ chọn"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:56
 #: openassessment/templates/openassessmentblock/oa_rubric.html:13
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:93
 #: openassessment/xblock/studio_mixin.py:47
 msgid "Required"
-msgstr ""
+msgstr "Bắt buộc"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:61
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:3
 msgid "Open Response Assessment"
-msgstr ""
+msgstr "Đánh Giá Câu Trả Lời Mở"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:8
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:7
 msgid "Prompt"
-msgstr ""
+msgstr "Gợi ý"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:15
 msgid "Rubric"
-msgstr ""
+msgstr "Phiếu tự đánh giá"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:22
 msgid "Schedule"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr "Налаштування"
+msgstr "Thiết lập"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
-msgstr ""
+msgstr "Tùy chọn"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
-msgstr ""
+msgstr "Lựa chọn Name"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:29
 msgid "Option Points"
-msgstr ""
+msgstr "Lựa chọn điểm"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:42
 msgid "Option Explanation"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:10
 msgid "Step: Peer Assessment"
-msgstr "Крок: Оцінювання студентами"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:15
 msgid ""
 "Peer Assessment allows students to provide feedback to other students and "
 "also receive feedback from others in their final grade. Often, though not "
 "always, this step is preceded by Self Assessment or Learner Training steps."
 msgstr ""
@@ -453,15 +458,15 @@
 msgid ""
 "Specify the number of peer assessments that each learner must complete. "
 "Valid numbers are 1 to 99."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:36
 msgid "Graded By"
-msgstr ""
+msgstr "Đã được phân loại theo"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:39
 msgid ""
 "Specify the number of learners that each response must be assessed by. Valid"
 " numbers are 1 to 99."
 msgstr ""
 
@@ -478,35 +483,35 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:5
 msgid "Peer Assessment Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:10
 msgid "Start Date"
-msgstr ""
+msgstr "Ngày bắt đầu"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:19
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:19
 msgid "Start Time"
-msgstr ""
+msgstr "Thời gian bắt đầu"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:119
 msgid "Due Date"
-msgstr "Кінцева дата"
+msgstr "Hạn nộp bài"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:40
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:40
 msgid "Due Time"
-msgstr ""
+msgstr "Thời Gian Tới Hạn"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:48
 msgid "The date and time when all peer assessments must be complete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:8
 msgid "You cannot delete a prompt after the assignment has been released."
@@ -516,15 +521,15 @@
 msgid ""
 "Prompts. Replace the sample text with your own text. For more information, "
 "see the ORA documentation."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html:22
 msgid "Add Prompt"
-msgstr ""
+msgstr "Thêm gợi ý"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:14
 msgid ""
 "Rubrics are made up of criteria, which usually contain one or more options. "
 "Each option has a point value. This template contains two sample criteria "
 "and their options. Replace the sample text with your own text. For more "
 "information, see the ORA documentation."
@@ -546,15 +551,15 @@
 msgid ""
 "Encourage learners to provide feedback on the response they have graded. You"
 " can replace the sample text with your own."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:49
 msgid "Default Feedback Text"
-msgstr ""
+msgstr "Mặc định Phản hồi văn bản"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:53
 msgid ""
 "Enter feedback text that learners will see before they enter their own "
 "feedback. Use this text to show learners a good example peer assessment."
 msgstr ""
 
@@ -584,15 +589,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:65
 msgid "The date and time when learners can no longer submit responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html:8
 msgid "Step: Self Assessment"
-msgstr ""
+msgstr "Bước: Tự đánh giá"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html:12
 msgid ""
 "Self Assessment asks learners to grade their own submissions against the "
 "rubric."
 msgstr ""
 
@@ -679,29 +684,29 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:7
 msgid "Scored Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
-msgstr ""
+msgstr "Điểm phản ứng"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr "Відповідь"
+msgstr "Trả Lời"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
-msgstr ""
+msgstr "Không Được Chọn"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:128
 msgid "points"
-msgstr ""
+msgstr "điểm"
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
@@ -714,64 +719,61 @@
 "                      %(assessment_title)s - %(points)s point\n"
 "                  "
 msgid_plural ""
 "\n"
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:24
 #, python-format
 msgid "More information about %(name)s"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
 msgid "Your Grade"
-msgstr ""
+msgstr "Điểm của bạn"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:19
 #, python-format
 msgid ""
 "\n"
 "                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:38
 msgid "Your submission has been cancelled."
-msgstr ""
+msgstr "Bài nộp của bạn đã bị hủy."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:19
 #, python-format
 msgid ""
 "\n"
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr "Ваша відповідь "
+msgstr "Trả Lời Của Bạn"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
-msgstr ""
+msgstr "Đánh Giá Trả Lời Của Bạn"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:50
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:132
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:28
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:28
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:4
 #: openassessment/templates/openassessmentblock/message/oa_message_closed.html:4
@@ -789,32 +791,32 @@
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:30
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:27
 msgid "Status"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:65
 msgid "Overall Grade"
-msgstr ""
+msgstr "Tổng điểm"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:70
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:28
 msgid "Points"
-msgstr ""
+msgstr "Điểm"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:96
 msgid "Additional comments on your response"
-msgstr ""
+msgstr "Nhận xét bổ sung về câu trả lời của bạn"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:117
 msgid "Provide feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:126
 msgid "Submitting Feedback"
-msgstr ""
+msgstr "Đang gửi phản hồi"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:134
 msgid ""
 "Your feedback has been submitted. Course staff will be able to see this "
 "feedback when they review course records."
 msgstr ""
 
@@ -828,64 +830,64 @@
 msgid ""
 "Select the statements below that best reflect your experience with peer "
 "assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:155
 msgid "These assessments were useful."
-msgstr ""
+msgstr "Những đánh giá này hữu ích."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:164
 msgid "These assessments were not useful."
-msgstr ""
+msgstr "Những đánh giá này không hữu ích."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:173
 msgid "I disagree with one or more of the peer assessments of my response."
-msgstr ""
+msgstr "Tôi không đồng tình với một hay các đánh giá của học viên khác về câu trả lời của mình."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:182
 msgid "Some comments I received were inappropriate."
-msgstr ""
+msgstr "Một số ý kiến ​​tôi nhận được không phù hợp."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:187
 msgid ""
 "Provide feedback on the grade or comments that you received from your peers."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:190
 msgid "I feel the feedback I received was..."
-msgstr ""
+msgstr "Tôi cảm thấy những phản hồi tôi nhận được ..."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:200
 msgid "We could not submit your feedback"
-msgstr ""
+msgstr "Chúng tôi không thể gửi phản hồi của bạn"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr ""
+msgstr "Chưa hoàn thành"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
-msgstr ""
+msgstr "Bạn chưa hoàn thành tất cả các bước của vấn đề này. "
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
-msgstr ""
+msgstr "Chưa bắt đầu"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:27
 msgid "You have not started this problem yet."
-msgstr ""
+msgstr "Bạn chưa bắt đầu bài này."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:16
 msgid "Waiting for Assessments"
-msgstr ""
+msgstr "Đang chờ đánh giá "
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:33
 msgid ""
 "You have completed your steps in the assignment, but some assessments still "
 "need to be done on your response. When the assessments of your response are "
 "complete, you will see feedback from everyone who assessed your response, "
 "and you will receive your final grade."
@@ -917,15 +919,15 @@
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:20
 #, python-format
 msgid "%(num_points)s points"
-msgstr ""
+msgstr "%(num_points)s điểm"
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:24
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:74
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:53
 msgid "Your peer's response to the prompt above"
 msgstr ""
 
@@ -1067,46 +1069,46 @@
 "\n"
 "                    This assignment has several steps. In the first step, you'll provide a response to the prompt. The other steps appear below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:4
 msgid "Instructions Unavailable"
-msgstr ""
+msgstr "Hướng dẫn không có sẵn"
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:6
 msgid "The instructions for this step could not be loaded."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:15
 msgid ""
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
-msgstr ""
+msgstr "Đang tải"
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
 msgid "Preview in LaTeX"
-msgstr "Попередній перегляд у LaTeX"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:10
 msgid "Click to preview your submission in LaTeX."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:15
 msgid "Preview Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
-msgstr ""
+msgstr "Nhận xét"
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
@@ -1209,24 +1211,24 @@
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr ""
+msgstr "Đã hoàn tất"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
 "Completing additional assessments will not affect your final grade."
-msgstr ""
+msgstr "Bạn đã hoàn thành tất cả các đánh giá ngang hàng cần thiết cho bài tập này. Bạn có thể đánh giá thêm câu trả lời của các học viên khác nếu muốn. Việc làm thêm đánh giá sẽ không ảnh hướng tới điểm số cuối cùng của bạn."
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:36
 msgid "We could not retrieve additional submissions for assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:43
 msgid "Continue Assessing Peers"
@@ -1250,15 +1252,15 @@
 #: openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html:16
 #: openassessment/templates/openassessmentblock/response/oa_response_unavailable.html:17
 #: openassessment/templates/openassessmentblock/self/oa_self_unavailable.html:17
 #: openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html:16
 #: openassessment/xblock/staff_assessment_mixin.py:165
 #: openassessment/xblock/staff_assessment_mixin.py:189
 msgid "Not Available"
-msgstr ""
+msgstr "Không có sẵn"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html:20
 #, python-format
 msgid ""
 "\n"
 "          In Progress (%(review_number)s of %(num_must_grade)s)\n"
 "        "
@@ -1297,15 +1299,15 @@
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
-msgstr ""
+msgstr "Trong tiến trình"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
@@ -1336,19 +1338,19 @@
 "                        You can save your progress and return to complete your response at any time before the due date\n"
 "                      "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:104
 msgid ""
 "You can save your progress and return to complete your response at any time."
-msgstr ""
+msgstr "Bạn có thể bảo lưu tiến độ của mình và quay lại để hoàn thành câu trả lời bất cứ lúc nào."
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:106
 msgid "After you submit your response, you cannot edit it"
-msgstr ""
+msgstr "Bạn sẽ không thể sửa câu trả lời sau khi gửi. "
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:116
 msgid "What will this assignment be graded on?"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:130
 msgid "The prompt for this section"
@@ -1415,23 +1417,23 @@
 "                                      You will not be part of Team %(team_name)s’s submission for this assignment and will not\n"
 "                                      receive a grade for their submission.\n"
 "                                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:221
 msgid "We could not save your progress"
-msgstr ""
+msgstr "Chúng tôi không thể lưu tiến độ của bạn"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:228
 msgid "Save your progress"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:232
 msgid "Your Submission Status"
-msgstr ""
+msgstr "Tình trạng gửi đi"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:242
 msgid "File Uploads "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:250
 msgid ""
@@ -1467,15 +1469,15 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:284
 msgid "Upload file"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:300
 msgid "You may continue to work on your response until you submit it."
-msgstr ""
+msgstr "Bạn có thể tiếp tục làm cho đến khi gửi bài."
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:306
 msgid "This is a team submission."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:308
 msgid ""
@@ -1507,15 +1509,15 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:334
 msgid "Submit your response and move to the next step"
-msgstr ""
+msgstr "Gửi trả lời của bạn và chuyển sang bước tiếp theo"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:34
 msgid "Your submission was cancelled. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:37
 #, python-format
@@ -1535,21 +1537,21 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:48
 #, python-format
 msgid ""
 "\n"
 "                            Comments: %(comments)s\n"
 "                        "
-msgstr ""
+msgstr "\n Bình luận: %(comments)s \n                        "
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:19
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:20
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
-msgstr ""
+msgstr "Chưa hoàn thành"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
@@ -1558,21 +1560,21 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:20
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:20
 #: openassessment/templates/openassessmentblock/self/oa_self_complete.html:18
 #: openassessment/templates/openassessmentblock/student_training/student_training_complete.html:17
 #: openassessment/xblock/staff_assessment_mixin.py:179
 #: openassessment/xblock/staff_assessment_mixin.py:202
 msgid "Complete"
-msgstr ""
+msgstr "Hoàn tất"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:51
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:57
 msgid "Your response"
-msgstr "Ваша відповідь"
+msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:33
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:54
 msgid "Your Uploaded Files"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:32
@@ -1618,15 +1620,15 @@
 "                            a response to this assignment with another team. Please contact course staff to discuss your\n"
 "                            options for this assignment.\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:23
 msgid "Assess Your Response"
-msgstr ""
+msgstr "Đánh giá phản hồi của bạn"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:31
 #, python-format, python-brace-format
 msgid ""
@@ -1700,49 +1702,49 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:52
 msgid "Enter a team member's username or edX email"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:56
 msgid "Submit"
-msgstr "Надіслати"
+msgstr "Gửi"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:78
 msgid "Response total"
-msgstr ""
+msgstr "Tổng phản hồi"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:84
 msgid "Location"
-msgstr ""
+msgstr "Địa chỉ"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:90
 msgid "Learner Progress"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:94
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:117
 msgid "Problem Step"
-msgstr ""
+msgstr "Các bước của vấn đề"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:95
 msgid "Active Learners in Step"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:113
 msgid "Dates"
-msgstr ""
+msgstr "Ngày"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:118
 msgid "Release Date"
-msgstr ""
+msgstr "Ngày phát hành"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:131
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:137
 msgid "N/A"
-msgstr ""
+msgstr "Không áp dụng"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
@@ -1913,17 +1915,14 @@
 "                                        %(assessment_label)s - %(points)s point\n"
 "                                    "
 msgid_plural ""
 "\n"
 "                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
 msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:165
 msgid "The submission is waiting for assessments."
@@ -1998,19 +1997,19 @@
 msgid ""
 "Removing a team's submission cannot be undone and should be done with "
 "caution."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:252
 msgid "Comments:"
-msgstr ""
+msgstr "Bình luận:"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:261
 msgid "Remove submission"
-msgstr ""
+msgstr "Gỡ bỏ bài nộp"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:276
 msgid "A response was not found for this learner."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:16
 #, python-format
@@ -2026,23 +2025,23 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:26
 msgid "Selected Option"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
-msgstr ""
+msgstr "Phản hồi"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
-msgstr ""
+msgstr "Tìm hiểu để đánh giá phản hồi"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:27
 #, python-format
 msgid ""
 "\n"
 "                      In Progress (%(current_progress_num)s of %(training_available_num)s)\n"
 "                  "
@@ -2110,15 +2109,15 @@
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:108
 msgid ""
 "The option you selected is not the option that the instructor selected."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:144
 msgid "We could not check your assessment"
-msgstr ""
+msgstr "Chúng tôi không thể kiểm tra đánh giá của bạn"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:151
 msgid "Compare your selections with the instructor's selections"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:29
 msgid ""
@@ -2149,31 +2148,31 @@
 
 #: openassessment/xblock/grade_mixin.py:77
 #: openassessment/xblock/leaderboard_mixin.py:61
 #: openassessment/xblock/self_assessment_mixin.py:42
 #: openassessment/xblock/student_training_mixin.py:56
 #: openassessment/xblock/student_training_mixin.py:264
 msgid "An unexpected error occurred."
-msgstr ""
+msgstr "Đã xảy ra lỗi không mong muốn."
 
 #: openassessment/xblock/grade_mixin.py:175
 msgid "Peer Assessment"
-msgstr "Оцінювання студентами"
+msgstr "Đánh giá giữa các học viên"
 
 #: openassessment/xblock/grade_mixin.py:177
 msgid "Self Assessment"
-msgstr ""
+msgstr "Tự Đánh Giá"
 
 #: openassessment/xblock/grade_mixin.py:217
 msgid "Assessment feedback could not be saved."
-msgstr ""
+msgstr "Phản hồi đánh giá không được lưu."
 
 #: openassessment/xblock/grade_mixin.py:228
 msgid "Feedback saved."
-msgstr ""
+msgstr "Phản hồi lưu."
 
 #: openassessment/xblock/grade_mixin.py:362
 #: openassessment/xblock/grade_mixin.py:508
 msgid "Staff Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:368
@@ -2192,28 +2191,28 @@
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Self Assessment Grade"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Your Self Assessment"
-msgstr ""
+msgstr "Tự đánh giá"
 
 #: openassessment/xblock/grade_mixin.py:385
 #: openassessment/xblock/grade_mixin.py:527
 msgid "Your Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:481
 msgid "Waiting for peer reviews"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:520
 msgid "Peer"
-msgstr ""
+msgstr "Bạn học"
 
 #: openassessment/xblock/grade_mixin.py:651
 msgid "The grade for this problem is determined by your Staff Grade."
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:653
 msgid ""
@@ -2262,29 +2261,29 @@
 msgid "You must submit a response before you can perform a peer assessment."
 msgstr ""
 
 #: openassessment/xblock/peer_assessment_mixin.py:73
 msgid ""
 "This feedback has already been submitted or the submission has been "
 "cancelled."
-msgstr ""
+msgstr "Thông tin phản hồi này đã được gửi hoặc việc nộp đã bị hủy."
 
 #: openassessment/xblock/peer_assessment_mixin.py:99
 #: openassessment/xblock/peer_assessment_mixin.py:105
 msgid "Your peer assessment could not be submitted."
-msgstr ""
+msgstr "Phần đánh giá giữa các học viên của bạn không thể được nộp."
 
 #: openassessment/xblock/peer_assessment_mixin.py:120
 #: openassessment/xblock/student_training_mixin.py:270
 msgid "Could not update workflow status."
-msgstr ""
+msgstr "Không thể cập nhật trạng thái công việc."
 
 #: openassessment/xblock/peer_assessment_mixin.py:128
 msgid "Could not load peer assessment."
-msgstr ""
+msgstr "Không thể tải đánh giá giữa các học viên."
 
 #: openassessment/xblock/peer_assessment_mixin.py:215
 msgid "Submit your assessment and review another response"
 msgstr ""
 
 #: openassessment/xblock/peer_assessment_mixin.py:219
 msgid "Submit your assessment and move to next step"
@@ -2338,28 +2337,28 @@
 #, python-brace-format
 msgid ""
 "No Open Response Assessment found in {course_id} with block id {block_id}"
 msgstr ""
 
 #: openassessment/xblock/self_assessment_mixin.py:142
 msgid "You must submit a response before you can perform a self-assessment."
-msgstr ""
+msgstr "Bạn phải nộp một phản hồi trước khi bạn có thể thực hiện tự đánh giá."
 
 #: openassessment/xblock/self_assessment_mixin.py:165
 #: openassessment/xblock/self_assessment_mixin.py:173
 msgid "Your self assessment could not be submitted."
-msgstr ""
+msgstr "Tự đánh giá của bạn không thể được nộp."
 
 #: openassessment/xblock/staff_area_mixin.py:42
 msgid "You do not have permission to schedule training"
-msgstr ""
+msgstr "Bạn không có quyền để lên lịch đào tạo"
 
 #: openassessment/xblock/staff_area_mixin.py:43
 msgid "You do not have permission to reschedule tasks."
-msgstr ""
+msgstr "Bạn không có quyền để sắp xếp lại các nhiệm vụ."
 
 #: openassessment/xblock/staff_area_mixin.py:69
 msgid "You do not have permission to access the ORA staff area"
 msgstr ""
 
 #: openassessment/xblock/staff_area_mixin.py:70
 msgid "You do not have permission to access ORA learner information."
@@ -2502,15 +2501,15 @@
 msgid ""
 "Error: When File Upload Response is disabled, Text Response must be Required"
 msgstr ""
 
 #: openassessment/xblock/studio_mixin.py:272
 #, python-brace-format
 msgid "Validation error: {error}"
-msgstr ""
+msgstr "Xác nhận lỗi: {error}"
 
 #: openassessment/xblock/studio_mixin.py:303
 msgid "Successfully updated OpenAssessment XBlock"
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:118
 msgid "\"submission\" required to submit answer."
@@ -2540,19 +2539,19 @@
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:261
 msgid "This response could not be saved."
-msgstr ""
+msgstr "Không thể lưu câu trả lời này."
 
 #: openassessment/xblock/submission_mixin.py:265
 msgid "This response was not submitted."
-msgstr ""
+msgstr "Phản hồi này đã không được gửi."
 
 #: openassessment/xblock/submission_mixin.py:281
 msgid "Files descriptions were not submitted."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:320
 msgid "Files metadata could not be saved."
@@ -2570,45 +2569,45 @@
 msgid ""
 "File upload failed: unsupported file type.Only the supported file types can "
 "be uploaded.If you have questions, please reach out to the course team."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:508
 msgid "Error retrieving upload URL."
-msgstr ""
+msgstr "Lỗi truy xuất URL tải lên."
 
 #: openassessment/xblock/submission_mixin.py:790
 msgid "This response has been saved but not submitted."
-msgstr ""
+msgstr "Câu trả lời này đã được lưu nhưng chưa được gửi đi."
 
 #: openassessment/xblock/submission_mixin.py:791
 msgid "This response has not been saved."
-msgstr ""
+msgstr "Câu trả lời này chưa được lưu."
 
 #: openassessment/xblock/validation.py:118
 msgid "This problem must include at least one assessment."
-msgstr ""
+msgstr "Vấn đề này phải bao gồm ít nhất một đánh giá."
 
 #: openassessment/xblock/validation.py:122
 msgid "The assessment order you selected is invalid."
-msgstr ""
+msgstr "Trình tự đánh giá bạn chọn không hợp lệ."
 
 #: openassessment/xblock/validation.py:132
 msgid "In peer assessment, the \"Must Grade\" value must be a positive integer."
 msgstr ""
 
 #: openassessment/xblock/validation.py:135
 msgid "In peer assessment, the \"Graded By\" value must be a positive integer."
-msgstr ""
+msgstr "Trong đánh phần giá giữa các học viên, giá trị \"được phân loại bởi \" phải là một số nguyên dương."
 
 #: openassessment/xblock/validation.py:139
 msgid ""
 "In peer assessment, the \"Must Grade\" value must be greater than or equal "
 "to the \"Graded By\" value."
-msgstr ""
+msgstr "Trong đánh phần giá giữa các học viên, giá trị của mục \"Phải được phân loại bởi\" phải lớn hơn hoặc bằng với giá trị  của \"được phân loại bởi \"."
 
 #: openassessment/xblock/validation.py:148
 msgid "You must provide at least one example response for learner training."
 msgstr ""
 
 #: openassessment/xblock/validation.py:151
 msgid "Each example response for learner training must be unique."
@@ -2668,8 +2667,8 @@
 
 #: openassessment/xblock/validation.py:356
 msgid "Leaderboard number is invalid."
 msgstr ""
 
 #: openassessment/xblock/validation.py:379
 msgid "The submission format is invalid."
-msgstr ""
+msgstr "Các định dạng cảu bài gửi không hợp lệ."
```

### Comparing `ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/uk/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# dangitdang <dangpham@mit.edu>, 2014
-# Doan Viet Hung <viethung.doan@gmail.com>, 2014
-# Duong Nguyen <supermanikin@yahoo.com>, 2015
-# Hoà Lê Thanh <hoa.lethanh@gmail.com>, 2017
-# Hoang Ha <halink0803@gmail.com>, 2014
-# hung nguyen <nguyenhungblog@gmail.com>, 2017
-# Le Minh Tri <trilm@hihexa.com>, 2020
-# Lê Như Ý <nhuyle89@gmail.com>, 2014
-# Minh Tue Vo <mvo@edx.org>, 2014
-# NGUYEN CONG NAM <congnam0409@gmail.com>, 2014
-# NGUYEN HOANG AN <neyugn2909@gmail.com>, 2014
-# Lam Nguyen <lamnguyen.cis@gmail.com>, 2020
-# Nguyen Nhat Quang <technicalmanager@gmail.com>, 2016
-# Sarina Canelake <sarina@tcril.org>, 2014
-# Thi Thanh Nga Do <thanhnga.ftu2@gmail.com>, 2015
-# Theodora. Tôn Nữ Quý Thiện <thien.tonnu1001@gmail.com>, 2015
-# Trần Tử Thiêng <trantuthieng26256@gmail.com>, 2014
-# Trung V. Nguyen <trung.ngvan@gmail.com>, 2015
-# Vinh Nguyen <vinhmaivy@gmail.com>, 2016
+# LIU,SHU-HAO <jeremy55662004@gmail.com>, 2014
+# JEN-HAO HSIEH <orienthauz@gmail.com>, 2015
+# Julia Oppenheimer <juliaoppenheimer2017@gmail.com>, 2019
+# KUN-MIN SYU <qwer20108@gmail.com>, 2014-2015
+# Lin Yu-Chun <iftwoplustwoequalsfive@gmail.com>, 2014
+# LIU,SHU-HAO <jeremy55662004@gmail.com>, 2014
+# MOH CHIN LAM <chinlam91@gmail.com>, 2015
+# Mose Chen <mosechen@gmail.com>, 2017
+# 2330b04c45946dd039e607f0ad907067_c74de22, 2014
+# vincent <orzkng2007@yahoo.com.tw>, 2015-2016
+# Wun-Han Syu <whsyu@mail.fcu.edu.tw>, 2016
+# Xaver Y.R. Chen <yrchen@atcity.org>, 2014-2016
+# Ya-chi Chang <yacchang@mail.fcu.edu.tw>, 2016
+# Ya-chi Chang <yacchang@mail.fcu.edu.tw>, 2016
+# Yenling Chen <bugchen.chen@gmail.com>, 2015-2016
+# Yung Wei <oscarwei1988@gmail.com>, 2016
+# Zhen-Rong Chen <zhenrc@gmail.com>, 2014
+# Zhen-Rong Chen <zhenrc@gmail.com>, 2014
+# KUN-MIN SYU <qwer20108@gmail.com>, 2014
+# 薛念林 <nlhsueh@mail.fcu.edu.tw>, 2016
+# 黃蕙君 <huanghc@mail.fcu.edu.tw>, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Lam Nguyen <lamnguyen.cis@gmail.com>, 2020\n"
-"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
+"Last-Translator: 黃蕙君 <huanghc@mail.fcu.edu.tw>, 2020\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: vi\n"
+"Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
 msgid "Could not parse serialized rubric"
-msgstr ""
+msgstr "系統無法解析 rubric "
 
 #: openassessment/assessment/api/student_training.py:191
 msgid ""
 "If your assignment includes a learner training step, the rubric must have at"
 " least one criterion, and that criterion must have at least one option."
-msgstr ""
+msgstr "如果您的任務包含一個評分訓練的步驟，則評分準則必須至少要有一個評分標準，並且那評分標準必須至少含一評分選項。"
 
 #: openassessment/assessment/api/student_training.py:203
 #, python-brace-format
 msgid "Example {example_number} has a validation error: {error}"
-msgstr "Ví dụ {example_number} có một lỗi xác nhận: {error}"
+msgstr "範例 {example_number} 出現驗證錯誤: {error}"
 
 #: openassessment/assessment/api/student_training.py:217
 #, python-brace-format
 msgid ""
 "Example {example_number} has an invalid option for \"{criterion_name}\": "
 "\"{option_name}\""
-msgstr ""
+msgstr "樣例 {example_number} 對 \"{criterion_name}\" 存在無效評分選項: \"{option_name}\""
 
 #: openassessment/assessment/api/student_training.py:227
 #, python-brace-format
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
-msgstr ""
+msgstr "樣例 {example_number} 為 \"{criterion_name}\" 提供額外評分選項"
 
 #: openassessment/assessment/api/student_training.py:240
 #, python-brace-format
 msgid "Example {example_number} is missing an option for \"{criterion_name}\""
-msgstr ""
+msgstr "樣例 {example_number} 對 \"{criterion_name}\" 缺少一個評分選項"
 
 #: openassessment/data.py:533
 #, python-brace-format
 msgid "Criterion {number}: {label}"
 msgstr ""
 
 #: openassessment/data.py:535
@@ -120,15 +122,15 @@
 #: openassessment/data.py:918
 msgid "Anonymous Scorer Id"
 msgstr ""
 
 #: openassessment/data.py:920
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:59
 msgid "Overall Feedback"
-msgstr "Phản hồi tổng thể"
+msgstr "整體的反饋意見"
 
 #: openassessment/data.py:921
 msgid "Assessment Score Earned"
 msgstr ""
 
 #: openassessment/data.py:922
 msgid "Assessment Scored At"
@@ -160,31 +162,31 @@
 
 #: openassessment/data.py:1320
 msgid "No description provided."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:28
 msgid "Save"
-msgstr "Lưu"
+msgstr "儲存"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit.html:32
 msgid "Cancel"
-msgstr "Hủy bỏ"
+msgstr "取消"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html:6
 msgid ""
 "Open Response Assessments allow you to configure single or multiple steps in"
 " a rubric based open response assessment sequence. The steps available below"
 " can be enabled, disable, and ordered for a flexible set of pedagogical "
 "needs."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:5
 msgid "Display Name "
-msgstr "Hiểu thị tên"
+msgstr "顯示名稱"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:8
 msgid "The display name for this component."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:12
 msgid "Text Response"
@@ -222,23 +224,23 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:52
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:93
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:131
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:157
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:45
 msgid "False"
-msgstr "Sai"
+msgstr "否"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:53
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:94
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:132
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:158
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:46
 msgid "True"
-msgstr "Đúng"
+msgstr "是"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:56
 msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
@@ -253,50 +255,50 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:61
 msgid "Image Files"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:62
 msgid "Custom File Types"
-msgstr ""
+msgstr "自定義檔案類型"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:66
 msgid ""
 "Specify whether learners can submit files along with their text responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:70
 msgid "File Types"
-msgstr ""
+msgstr "檔案類型"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:79
 msgid ""
 "Enter the file extensions, separated by commas, that you want learners to be"
 " able to upload. For example: pdf,doc,docx."
-msgstr ""
+msgstr "輸入文件名，並用逗號分隔，您希望學習者能夠上傳。例如：PDF，DOC，DOCX。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:84
 msgid ""
 "To add more file extensions, select Custom File Types and enter the full "
 "list of acceptable file extensions to be included."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:91
 msgid "Allow LaTeX Responses"
-msgstr ""
+msgstr "允許Latex格式作答"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:97
 msgid "Specify whether learners can write LaTeX formatted strings"
-msgstr ""
+msgstr "是否要讓學生可以撰寫Latex格式的字串"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:102
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:8
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html:10
 msgid "Top Responses"
-msgstr ""
+msgstr "作業觀摩數"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:104
 msgid " (Disabled)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:117
 msgid ""
@@ -331,110 +333,110 @@
 "response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:6
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:122
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:25
 msgid "Criterion"
-msgstr ""
+msgstr "評分標準"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:7
 msgid "You cannot delete a criterion after the assignment has been released."
-msgstr ""
+msgstr "你不能夠在問題被釋出後刪除評分標準"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:9
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:7
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:10
 msgid "Remove"
-msgstr "Loại bỏ"
+msgstr "移除"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:17
 msgid "Criterion Name"
-msgstr ""
+msgstr "評分標準名稱"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:29
 msgid "Criterion Prompt"
-msgstr ""
+msgstr "評分標準描述"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:44
 msgid "Add Option"
-msgstr "Thêm Tùy chọn"
+msgstr "增加評分選項"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:52
 msgid "Feedback for This Criterion"
-msgstr ""
+msgstr "此評分標準的回饋"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:54
 #: openassessment/xblock/studio_mixin.py:49
 msgid "None"
-msgstr ""
+msgstr "無"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:55
 #: openassessment/xblock/studio_mixin.py:48
 msgid "Optional"
-msgstr "tuỳ chọn"
+msgstr "非必填"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:56
 #: openassessment/templates/openassessmentblock/oa_rubric.html:13
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:93
 #: openassessment/xblock/studio_mixin.py:47
 msgid "Required"
-msgstr "Bắt buộc"
+msgstr "需要評分"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:61
 msgid ""
 "Select one of the options above. This describes whether or not the reviewer "
 "will have to provide criterion feedback."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:3
 msgid "Open Response Assessment"
-msgstr "Đánh Giá Câu Trả Lời Mở"
+msgstr "開放式問題評分"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:8
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:7
 msgid "Prompt"
-msgstr "Gợi ý"
+msgstr "問題描述"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:15
 msgid "Rubric"
-msgstr "Phiếu tự đánh giá"
+msgstr "評分準則"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:22
 msgid "Schedule"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:29
 msgid "Assessment steps"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html:36
 msgid "Settings"
-msgstr "Thiết lập"
+msgstr "設定"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:5
 msgid "Option"
-msgstr "Tùy chọn"
+msgstr "評分選項"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:16
 msgid "Option Name"
-msgstr "Lựa chọn Name"
+msgstr "評分選項名稱"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:29
 msgid "Option Points"
-msgstr "Lựa chọn điểm"
+msgstr "評分選項點數"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_option.html:42
 msgid "Option Explanation"
-msgstr ""
+msgstr "評分選項說明"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:10
 msgid "Step: Peer Assessment"
-msgstr ""
+msgstr "步驟 : 同儕互評"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:15
 msgid ""
 "Peer Assessment allows students to provide feedback to other students and "
 "also receive feedback from others in their final grade. Often, though not "
 "always, this step is preceded by Self Assessment or Learner Training steps."
 msgstr ""
@@ -448,25 +450,25 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:23
 msgid "View Options & Configuration"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:29
 msgid "Must Grade"
-msgstr ""
+msgstr "必需評分數"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:32
 msgid ""
 "Specify the number of peer assessments that each learner must complete. "
 "Valid numbers are 1 to 99."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:36
 msgid "Graded By"
-msgstr "Đã được phân loại theo"
+msgstr "被評分數"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html:39
 msgid ""
 "Specify the number of learners that each response must be assessed by. Valid"
 " numbers are 1 to 99."
 msgstr ""
 
@@ -483,121 +485,121 @@
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:5
 msgid "Peer Assessment Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:10
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:10
 msgid "Start Date"
-msgstr "Ngày bắt đầu"
+msgstr "開始日期"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:19
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:19
 msgid "Start Time"
-msgstr "Thời gian bắt đầu"
+msgstr "開始時間"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:119
 msgid "Due Date"
-msgstr "Hạn nộp bài"
+msgstr "截止日期"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:40
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:40
 msgid "Due Time"
-msgstr "Thời Gian Tới Hạn"
+msgstr "截止時間"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html:48
 msgid "The date and time when all peer assessments must be complete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html:8
 msgid "You cannot delete a prompt after the assignment has been released."
-msgstr ""
+msgstr "注意，一旦發佈了此作業，此題目就無法刪除。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html:10
 msgid ""
 "Prompts. Replace the sample text with your own text. For more information, "
 "see the ORA documentation."
-msgstr ""
+msgstr "題目。取代下方範例文字，寫上你同儕互評的題目。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html:22
 msgid "Add Prompt"
-msgstr "Thêm gợi ý"
+msgstr "增加題目"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:14
 msgid ""
 "Rubrics are made up of criteria, which usually contain one or more options. "
 "Each option has a point value. This template contains two sample criteria "
 "and their options. Replace the sample text with your own text. For more "
 "information, see the ORA documentation."
-msgstr ""
+msgstr "評分準則由通常包含一個或多個評分選項的評分標準組成。每個評分選項有一個分數值。這個樣版中包含兩個範例評分標準以及他們的評分選項。將範例文字取代成你自己的文字。如果需要更多資訊，請看ORA的教學˙文件"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:29
 msgid "Add Criterion"
-msgstr ""
+msgstr "增加評分標準"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:35
 msgid "Feedback for This Response"
-msgstr ""
+msgstr "此作答的回饋"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:40
 msgid "Feedback Instructions"
-msgstr ""
+msgstr "回饋說明"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:44
 msgid ""
 "Encourage learners to provide feedback on the response they have graded. You"
 " can replace the sample text with your own."
-msgstr ""
+msgstr "鼓勵學習者提供對作答的回饋。您可以取代樣板文字，寫上您的您的意見。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:49
 msgid "Default Feedback Text"
-msgstr "Mặc định Phản hồi văn bản"
+msgstr "預設回饋文字"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html:53
 msgid ""
 "Enter feedback text that learners will see before they enter their own "
 "feedback. Use this text to show learners a good example peer assessment."
-msgstr ""
+msgstr "輸入樣板的作答回饋。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:5
 msgid "Course Deadlines"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:13
 msgid "Response Start Date"
-msgstr ""
+msgstr "作答開始日期"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:26
 msgid "Response Start Time"
-msgstr ""
+msgstr "作答開始時間"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:35
 msgid "The date and time when learners can begin submitting responses."
-msgstr ""
+msgstr "學生可以開始提交作答的日期及時間。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:43
 msgid "Response Due Date"
-msgstr ""
+msgstr "作答截止日期"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:56
 msgid "Response Due Time"
-msgstr ""
+msgstr "作答截止時間"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html:65
 msgid "The date and time when learners can no longer submit responses."
-msgstr ""
+msgstr "學生不能再提交作答的日期及時間。"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html:8
 msgid "Step: Self Assessment"
-msgstr "Bước: Tự đánh giá"
+msgstr "步驟 : 自我評量 "
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html:12
 msgid ""
 "Self Assessment asks learners to grade their own submissions against the "
 "rubric."
 msgstr ""
 
@@ -611,25 +613,25 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:48
 msgid "The date and time when all self assessments must be complete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html:8
 msgid "Step: Staff Assessment"
-msgstr ""
+msgstr "步驟：工作人員評估"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html:12
 msgid ""
 "Staff Assessment gates sets the final grade for students if enabled with "
 "other steps, though it can also be used as a standalone step."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:9
 msgid "Step: Learner Training"
-msgstr ""
+msgstr "步驟：評分訓練"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:14
 msgid ""
 "Learner Training is used to help students practice grading a simulated peer "
 "submission in order to train them on the rubric and ensure learner's "
 "understand the rubric for either Self or Peer Assessment steps."
 msgstr ""
@@ -644,15 +646,15 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:22
 msgid "View / Add Sample Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:32
 msgid "Add Sample Response"
-msgstr ""
+msgstr "新增範例作答"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:4
 msgid "Clone Rubric"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:7
 msgid ""
@@ -680,33 +682,33 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:37
 msgid "Rubric Successfully Cloned from Block ID: "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:7
 msgid "Scored Response"
-msgstr ""
+msgstr "作答與答案的分數"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
-msgstr "Điểm phản ứng"
+msgstr "作答評分"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:27
 msgid "Response"
-msgstr "Trả Lời"
+msgstr "作答"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:10
 msgid "Not Selected"
-msgstr "Không Được Chọn"
+msgstr "未選取"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html:15
 #: openassessment/templates/openassessmentblock/oa_rubric.html:43
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:128
 msgid "points"
-msgstr "điểm"
+msgstr "點數"
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html:8
 #, python-format
 msgid ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - %(grade)s%(end_tag)s\n"
 "              "
@@ -723,57 +725,57 @@
 "                      %(assessment_title)s - %(points)s points\n"
 "                  "
 msgstr[0] ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_assessment_title.html:24
 #, python-format
 msgid "More information about %(name)s"
-msgstr ""
+msgstr "更多訊息關於 %(name)s"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:15
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:26
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:14
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:14
 msgid "Your Grade"
-msgstr "Điểm của bạn"
+msgstr "您的成績"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:19
 #, python-format
 msgid ""
 "\n"
 "                                        %(points_earned)s out of %(points_possible)s\n"
 "                                    "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html:38
 msgid "Your submission has been cancelled."
-msgstr "Bài nộp của bạn đã bị hủy."
+msgstr "您的提交已經被取消。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:19
 #, python-format
 msgid ""
 "\n"
 "                                            %(points_earned)s out of %(points_possible)s\n"
 "                                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:38
 #: openassessment/templates/openassessmentblock/response/oa_response.html:29
 msgid "Your Response"
-msgstr "Trả Lời Của Bạn"
+msgstr "您的作答"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:41
 msgid "Your Upload"
-msgstr ""
+msgstr "你的上傳"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:46
 msgid "Assessments of Your Response"
-msgstr "Đánh Giá Trả Lời Của Bạn"
+msgstr "對您作答的評分。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:50
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:132
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:28
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:28
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:4
 #: openassessment/templates/openassessmentblock/message/oa_message_closed.html:4
@@ -791,103 +793,103 @@
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:30
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:27
 msgid "Status"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:65
 msgid "Overall Grade"
-msgstr "Tổng điểm"
+msgstr "整體成績"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:70
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:28
 msgid "Points"
-msgstr "Điểm"
+msgstr "點數"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:96
 msgid "Additional comments on your response"
-msgstr "Nhận xét bổ sung về câu trả lời của bạn"
+msgstr "對您作答的額外評論"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:117
 msgid "Provide feedback on peer assessments"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:126
 msgid "Submitting Feedback"
-msgstr "Đang gửi phản hồi"
+msgstr "提交反饋意見"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:134
 msgid ""
 "Your feedback has been submitted. Course staff will be able to see this "
 "feedback when they review course records."
-msgstr ""
+msgstr "您的反饋意見已經被提交。課程職員將會在他們檢查課程記錄時看到這條反饋意見"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:140
 msgid ""
 "Course staff will be able to see any feedback that you provide here when "
 "they review course records."
-msgstr ""
+msgstr "當課程工作人員審核課程記錄時，他們可以查看您發表於此的所有反饋意見內容。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:146
 msgid ""
 "Select the statements below that best reflect your experience with peer "
 "assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:155
 msgid "These assessments were useful."
-msgstr "Những đánh giá này hữu ích."
+msgstr "這些評分很有用。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:164
 msgid "These assessments were not useful."
-msgstr "Những đánh giá này không hữu ích."
+msgstr "這些評分沒有用。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:173
 msgid "I disagree with one or more of the peer assessments of my response."
-msgstr "Tôi không đồng tình với một hay các đánh giá của học viên khác về câu trả lời của mình."
+msgstr "我不同意同儕對我答案的一份或者多份評分。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:182
 msgid "Some comments I received were inappropriate."
-msgstr "Một số ý kiến ​​tôi nhận được không phù hợp."
+msgstr "我收到的某些評論並不合適。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:187
 msgid ""
 "Provide feedback on the grade or comments that you received from your peers."
-msgstr ""
+msgstr "針對同儕給予的分數或意見提供回饋。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:190
 msgid "I feel the feedback I received was..."
-msgstr "Tôi cảm thấy những phản hồi tôi nhận được ..."
+msgstr "我感覺我收到的反饋意見很..."
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:200
 msgid "We could not submit your feedback"
-msgstr "Chúng tôi không thể gửi phản hồi của bạn"
+msgstr "我們無法提交您的反饋意見"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_complete.html:206
 msgid "Submit feedback on peer assessments"
-msgstr ""
+msgstr "針對同儕互評提交回饋"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:16
 msgid "Not Completed"
-msgstr "Chưa hoàn thành"
+msgstr "未完成"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html:33
 msgid "You have not completed all the steps of this problem."
-msgstr "Bạn chưa hoàn thành tất cả các bước của vấn đề này. "
+msgstr "您還沒有完成這個問題的所有步驟。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:16
 msgid "Not Started"
-msgstr "Chưa bắt đầu"
+msgstr "未開始"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html:27
 msgid "You have not started this problem yet."
-msgstr "Bạn chưa bắt đầu bài này."
+msgstr "您還沒有開始這個問題。"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:16
 msgid "Waiting for Assessments"
-msgstr "Đang chờ đánh giá "
+msgstr "正在等待評量"
 
 #: openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html:33
 msgid ""
 "You have completed your steps in the assignment, but some assessments still "
 "need to be done on your response. When the assessments of your response are "
 "complete, you will see feedback from everyone who assessed your response, "
 "and you will receive your final grade."
@@ -919,27 +921,27 @@
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:20
 #, python-format
 msgid "%(num_points)s points"
-msgstr "%(num_points)s điểm"
+msgstr "%(num_points)s 點"
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:24
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:74
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:53
 msgid "Your peer's response to the prompt above"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html:19
 msgid ""
 "After you complete all the steps of this assignment, you can see the top-"
 "scoring responses from your peers."
-msgstr ""
+msgstr "當你完成所有評分的步驟後，你將可以看到同學們中較佳的作答"
 
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:8
 msgid ""
 "Your team’s submission has been cancelled. Your team will receive a grade of"
 " zero unless course staff resets your assessment to allow the team to "
 "resubmit a response."
 msgstr ""
@@ -1069,46 +1071,46 @@
 "\n"
 "                    This assignment has several steps. In the first step, you'll provide a response to the prompt. The other steps appear below the %(start_tag)sYour Response%(end_tag)s field.\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:4
 msgid "Instructions Unavailable"
-msgstr "Hướng dẫn không có sẵn"
+msgstr "找不到說明"
 
 #: openassessment/templates/openassessmentblock/message/oa_message_unavailable.html:6
 msgid "The instructions for this step could not be loaded."
-msgstr ""
+msgstr "無法載入此步驟的說明"
 
 #: openassessment/templates/openassessmentblock/oa_base.html:15
 msgid ""
 "This assignment has several steps. In the first step, you'll provide a "
 "response to the prompt. The other steps appear below the Your Response "
 "field."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_base.html:36
 msgid "Loading"
-msgstr "Đang tải"
+msgstr "讀取中..."
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:7
 msgid "Preview in LaTeX"
-msgstr ""
+msgstr "Latex格式預覽"
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:10
 msgid "Click to preview your submission in LaTeX."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_latex_preview.html:15
 msgid "Preview Response"
-msgstr ""
+msgstr "預覽作答"
 
 #: openassessment/templates/openassessmentblock/oa_rubric.html:53
 msgid "Comments"
-msgstr "Nhận xét"
+msgstr "評論"
 
 #: openassessment/templates/openassessmentblock/oa_submission_answer.html:8
 msgid "The question for this section"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/oa_team_uploaded_files.html:8
 msgid "Files that were uploaded by your teammates:"
@@ -1132,15 +1134,15 @@
 "Caution: These files were uploaded by another course learner and have not "
 "been verified, screened, approved, reviewed, or endorsed by the site "
 "administrator. If you access the files, you do so at your own risk.)"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:26
 msgid "Assess Peers"
-msgstr ""
+msgstr "評量同儕"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 00:00 UTC (in
 #. 5 days and 45 minutes)"
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:34
 #, python-format, python-brace-format
 msgid ""
@@ -1167,15 +1169,15 @@
 "                    In Progress (%(review_number)s of %(num_must_grade)s)\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:65
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:45
 msgid "Read and assess the following response from one of your peers."
-msgstr ""
+msgstr "讀取並評量您的同儕送來的答案。"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:77
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:56
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:60
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:45
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:38
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:63
@@ -1184,83 +1186,83 @@
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html:91
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:70
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:71
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:57
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:50
 msgid "We could not submit your assessment"
-msgstr ""
+msgstr "我們無法提交您的評分。"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html:19
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:21
 #: openassessment/templates/openassessmentblock/self/oa_self_cancelled.html:21
 #: openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html:18
 #: openassessment/xblock/staff_assessment_mixin.py:172
 msgid "Cancelled"
-msgstr ""
+msgstr "取消"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html:20
 #, python-format
 msgid ""
 "\n"
 "            Incomplete (%(num_graded)s of %(num_must_grade)s)\n"
 "        "
-msgstr ""
+msgstr "\n未完成評分(%(num_must_grade)s of %(num_graded)s)"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_closed.html:35
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete peer assessments or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:13
 msgid "Completed"
-msgstr "Đã hoàn tất"
+msgstr "完成"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:31
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:41
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:36
 msgid ""
 "You have successfully completed all of the required peer assessments for "
 "this assignment. You may assess additional peer responses if you want to. "
 "Completing additional assessments will not affect your final grade."
-msgstr "Bạn đã hoàn thành tất cả các đánh giá ngang hàng cần thiết cho bài tập này. Bạn có thể đánh giá thêm câu trả lời của các học viên khác nếu muốn. Việc làm thêm đánh giá sẽ không ảnh hướng tới điểm số cuối cùng của bạn."
+msgstr "您已經成功完成所有作業中必須的同儕互評。若您想要的話，您可以進行更多的同儕互評。完成更多的評量將不會影響您的期末成績。"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:36
 msgid "We could not retrieve additional submissions for assessment"
-msgstr ""
+msgstr "我們不能檢索額外的提交評分"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_complete.html:43
 msgid "Continue Assessing Peers"
-msgstr ""
+msgstr "繼續評量同儕"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html:26
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:20
 #, python-format
 msgid ""
 "\n"
 "        Complete (%(num_graded)s)\n"
 "      "
-msgstr ""
+msgstr "\n完成 (%(num_graded)s)"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html:38
 msgid ""
 "All submitted peer responses have been assessed. Check back later to see if "
 "more learners have submitted responses."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html:16
 #: openassessment/templates/openassessmentblock/response/oa_response_unavailable.html:17
 #: openassessment/templates/openassessmentblock/self/oa_self_unavailable.html:17
 #: openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html:16
 #: openassessment/xblock/staff_assessment_mixin.py:165
 #: openassessment/xblock/staff_assessment_mixin.py:189
 msgid "Not Available"
-msgstr "Không có sẵn"
+msgstr "目前還未進入此階段"
 
 #: openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html:20
 #, python-format
 msgid ""
 "\n"
 "          In Progress (%(review_number)s of %(num_must_grade)s)\n"
 "        "
@@ -1299,15 +1301,15 @@
 "            <span id=\"oa_step_deadline_response\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:54
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:46
 msgid "In Progress"
-msgstr "Trong tiến trình"
+msgstr "正在進行中"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:66
 msgid "Enter your team's response to the prompt."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:68
 msgid ""
@@ -1338,19 +1340,19 @@
 "                        You can save your progress and return to complete your response at any time before the due date\n"
 "                      "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:104
 msgid ""
 "You can save your progress and return to complete your response at any time."
-msgstr "Bạn có thể bảo lưu tiến độ của mình và quay lại để hoàn thành câu trả lời bất cứ lúc nào."
+msgstr "您可以隨時儲存並回頭修改您的答案"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:106
 msgid "After you submit your response, you cannot edit it"
-msgstr "Bạn sẽ không thể sửa câu trả lời sau khi gửi. "
+msgstr "在您送出答案以後，您不能再修改它"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:116
 msgid "What will this assignment be graded on?"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:130
 msgid "The prompt for this section"
@@ -1417,23 +1419,23 @@
 "                                      You will not be part of Team %(team_name)s’s submission for this assignment and will not\n"
 "                                      receive a grade for their submission.\n"
 "                                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:221
 msgid "We could not save your progress"
-msgstr "Chúng tôi không thể lưu tiến độ của bạn"
+msgstr "我們無法儲存您的進度"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:228
 msgid "Save your progress"
-msgstr ""
+msgstr "儲存您的進度"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:232
 msgid "Your Submission Status"
-msgstr "Tình trạng gửi đi"
+msgstr "您的提交狀態"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:242
 msgid "File Uploads "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:250
 msgid ""
@@ -1453,15 +1455,15 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:271
 msgid "Select one or more files to upload for this submission."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:273
 msgid "Select a file to upload for this submission."
-msgstr ""
+msgstr "選擇本次提交上傳的檔案。"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:278
 msgid "Supported file types: "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:282
 msgid "Upload files"
@@ -1469,15 +1471,15 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:284
 msgid "Upload file"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:300
 msgid "You may continue to work on your response until you submit it."
-msgstr "Bạn có thể tiếp tục làm cho đến khi gửi bài."
+msgstr "您可以在送出答案前繼續工作"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:306
 msgid "This is a team submission."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:308
 msgid ""
@@ -1505,31 +1507,31 @@
 "\n"
 "                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
-msgstr ""
+msgstr "我們無法送出您的回應"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:334
 msgid "Submit your response and move to the next step"
-msgstr "Gửi trả lời của bạn và chuyển sang bước tiếp theo"
+msgstr "送出您的回應並移動至下一步"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:34
 msgid "Your submission was cancelled. "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:37
 #, python-format
 msgid ""
 "\n"
 "                                Your submission has been cancelled by %(removed_by_username)s on %(removed_datetime)s\n"
 "                            "
-msgstr ""
+msgstr "\n您的提交已經在%(removed_datetime)s被%(removed_by_username)s取消"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:41
 #, python-format
 msgid ""
 "\n"
 "                               Your submission was cancelled on %(removed_datetime)s\n"
 "                            "
@@ -1537,21 +1539,21 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response_cancelled.html:48
 #, python-format
 msgid ""
 "\n"
 "                            Comments: %(comments)s\n"
 "                        "
-msgstr "\n Bình luận: %(comments)s \n                        "
+msgstr "\n評論：%(comments)s"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:19
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:20
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:17
 msgid "Incomplete"
-msgstr "Chưa hoàn thành"
+msgstr "未完成"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer submit a response or continue with this problem, and you will receive"
 " a grade of Incomplete. If you saved but did not submit a response, the "
 "response appears in the course records."
@@ -1560,15 +1562,15 @@
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:20
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:20
 #: openassessment/templates/openassessmentblock/self/oa_self_complete.html:18
 #: openassessment/templates/openassessmentblock/student_training/student_training_complete.html:17
 #: openassessment/xblock/staff_assessment_mixin.py:179
 #: openassessment/xblock/staff_assessment_mixin.py:202
 msgid "Complete"
-msgstr "Hoàn tất"
+msgstr "完成"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_graded.html:30
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:51
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:57
 msgid "Your response"
 msgstr ""
 
@@ -1585,31 +1587,31 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:34
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(peer_start_tag)speer assessment%(end_tag)s and %(self_start_tag)sself assessment%(end_tag)s steps.\n"
 "                    "
-msgstr ""
+msgstr "\n你仍需要完成%(peer_start_tag)s同儕互評%(end_tag)s和%(self_start_tag)s自我評量%(end_tag)s的步驟。"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:38
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(start_tag)speer assessment%(end_tag)s step.\n"
 "                    "
-msgstr ""
+msgstr "\n你仍需要完成 %(start_tag)s同儕互評%(end_tag)s的步驟。"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_submitted.html:42
 #, python-format
 msgid ""
 "\n"
 "                        You still need to complete the %(start_tag)sself assessment%(end_tag)s step.\n"
 "                    "
-msgstr ""
+msgstr "\n你仍需要完成 %(start_tag)s自我評量%(end_tag)s的步驟。"
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:15
 msgid "Error"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html:29
 #, python-format
@@ -1620,15 +1622,15 @@
 "                            a response to this assignment with another team. Please contact course staff to discuss your\n"
 "                            options for this assignment.\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:23
 msgid "Assess Your Response"
-msgstr "Đánh giá phản hồi của bạn"
+msgstr "評量您的回應"
 
 #. Translators: This string displays a date to the user, then tells them the
 #. time until that date.  Example: "available August 13th, 2014 (in 5 days and
 #. 45 minutes)"
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:31
 #, python-format, python-brace-format
 msgid ""
@@ -1646,15 +1648,15 @@
 "\n"
 "               <span id=\"oa_step_deadline_self\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "           "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/self/oa_self_assessment.html:78
 msgid "Submit your assessment"
-msgstr ""
+msgstr "送出您的作答"
 
 #: openassessment/templates/openassessmentblock/self/oa_self_closed.html:32
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer complete a self assessment or continue with this assignment, and you "
 "will receive a grade of Incomplete."
 msgstr ""
@@ -1663,92 +1665,92 @@
 #: openassessment/xblock/grade_mixin.py:361
 msgid "Staff Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:8
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:35
 msgid "Manage Individual Learners"
-msgstr ""
+msgstr "管理個別學生"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:10
 msgid "Manage Team Responses"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:13
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:71
 msgid "View Assignment Statistics"
-msgstr ""
+msgstr "瀏覽作業統計"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:22
 msgid "Demo the new Grading Experience"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:26
 msgid "View ORA in Studio"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:69
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:151
 msgid "Close"
-msgstr ""
+msgstr "關閉"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:37
 msgid "Manage Teams"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:50
 msgid "Enter an individual learner's username or email"
-msgstr ""
+msgstr "輸入個別學生的使用者帳號或電子郵件信箱。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:52
 msgid "Enter a team member's username or edX email"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:56
 msgid "Submit"
-msgstr "Gửi"
+msgstr "提交"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:78
 msgid "Response total"
-msgstr "Tổng phản hồi"
+msgstr "回應總數"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:84
 msgid "Location"
-msgstr "Địa chỉ"
+msgstr "位置"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:90
 msgid "Learner Progress"
-msgstr ""
+msgstr "學生進度"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:94
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:117
 msgid "Problem Step"
-msgstr "Các bước của vấn đề"
+msgstr "問題步驟"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:95
 msgid "Active Learners in Step"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:113
 msgid "Dates"
-msgstr "Ngày"
+msgstr "日期"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:118
 msgid "Release Date"
-msgstr "Ngày phát hành"
+msgstr "釋出日期"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:131
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:137
 msgid "N/A"
-msgstr "Không áp dụng"
+msgstr "不適用"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
-msgstr ""
+msgstr "工作人員評估"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:16
 msgid "Give this learner a grade using the problem's rubric."
@@ -1765,39 +1767,39 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:30
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:20
 #, python-format
 msgid ""
 "\n"
 "                                        Response for: %(student_username)s\n"
 "                                    "
-msgstr ""
+msgstr "\n回應為：%(student_username)s"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:34
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:24
 msgid "Learner Response"
-msgstr ""
+msgstr "學生回應"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:39
 msgid "The teams's response to the prompt above"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:41
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:32
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:57
 msgid "The learner's response to the prompt above"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:64
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html:57
 msgid "Submit assessment"
-msgstr ""
+msgstr "送出測驗"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:70
 msgid "Submit assessment and continue grading"
-msgstr ""
+msgstr "提交評估和持續評分"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html:6
 #, python-format
 msgid ""
 "\n"
 "                %(ungraded)s Available and %(in_progress)s Checked Out\n"
 "            "
@@ -1834,67 +1836,67 @@
 "\n"
 "                    Viewing team: %(team)s\n"
 "                "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:28
 msgid "Learner's Response"
-msgstr ""
+msgstr "學習者的回應"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:30
 msgid "Team's Response"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:39
 #, python-format
 msgid ""
 "\n"
 "                            Learner submission removed by %(removed_by_username)s on %(removed_datetime)s\n"
 "                        "
-msgstr ""
+msgstr "\n學生所提交的已經在%(removed_datetime)s被%(removed_by_username)s移除"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:43
 #, python-format
 msgid ""
 "\n"
 "                            Learner submission removed on %(removed_datetime)s\n"
 "                        "
-msgstr ""
+msgstr "\n學習者提交解除%(removed_datetime)s"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:50
 #, python-format
 msgid ""
 "\n"
 "                        Comments: %(comments)s\n"
 "                    "
-msgstr ""
+msgstr "\n評論：%(comments)s"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:71
 msgid "Peer Assessments for This Learner"
-msgstr ""
+msgstr "針對此學生的同儕互評"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:76
 msgid "Peer Assessments Completed by This Learner"
-msgstr ""
+msgstr "此學生已完成的同儕互評"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:81
 msgid "Learner's Self Assessment"
-msgstr ""
+msgstr "學生的自我評量"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:87
 msgid "Staff Assessment for This Learner"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:89
 msgid "Staff Assessment for this Team"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:100
 msgid "Learner's Final Grade"
-msgstr ""
+msgstr "學習者最終的成績"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:102
 msgid "Team's Final Grade"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:112
 #, python-format
@@ -1902,35 +1904,35 @@
 "\n"
 "                            Final grade: %(points_earned)s out of %(points_possible)s\n"
 "                        "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:119
 msgid "Final Grade Details"
-msgstr ""
+msgstr "最終成績的詳細資料"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:139
 #, python-format
 msgid ""
 "\n"
 "                                        %(assessment_label)s - %(points)s point\n"
 "                                    "
 msgid_plural ""
 "\n"
 "                                        %(assessment_label)s - %(points)s points\n"
 "                                    "
-msgstr[0] ""
+msgstr[0] "\n%(assessment_label)s - %(points)s 分數"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:154
 msgid "Feedback Recorded"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:165
 msgid "The submission is waiting for assessments."
-msgstr ""
+msgstr "意見正在等待評量。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:170
 msgid ""
 "The learner's submission has been removed from peer assessment. The learner "
 "receives a grade of zero unless you delete the learner's state for the "
 "problem to allow them to resubmit a response."
 msgstr ""
@@ -1940,23 +1942,23 @@
 "The team’s submission has been removed from grading. The team receives a "
 "grade of zero unless you delete the a team member’s state for the problem to"
 " allow the team to resubmit a response."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:177
 msgid "The problem has not been started."
-msgstr ""
+msgstr "這個問題尚未開始"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:181
 msgid "The problem has not been completed."
-msgstr ""
+msgstr "問題尚未被完成。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:193
 msgid "Submit Assessment Grade Override"
-msgstr ""
+msgstr "提交覆蓋測驗評分"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:195
 msgid "Submit Team Grade Override"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:204
 msgid "Unable to perform grade override"
@@ -1973,75 +1975,75 @@
 "This submission has been cancelled and cannot recieve a grade. Refer to "
 "documentation for how to delete the learner’s state for this problem to "
 "allow them to resubmit."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:230
 msgid "Remove Submission From Peer Grading"
-msgstr ""
+msgstr "從同儕互評中移除提交"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:232
 msgid "Remove Team Submission from Grading"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:242
 msgid "Caution: This Action Cannot Be Undone"
-msgstr ""
+msgstr "注意: 必須完成此操作。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:244
 msgid ""
 "Removing a learner's submission cannot be undone and should be done with "
 "caution."
-msgstr ""
+msgstr "移除學習者的提交無法撤銷，應謹慎進行。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:246
 msgid ""
 "Removing a team's submission cannot be undone and should be done with "
 "caution."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:252
 msgid "Comments:"
-msgstr "Bình luận:"
+msgstr "評論："
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:261
 msgid "Remove submission"
-msgstr "Gỡ bỏ bài nộp"
+msgstr "移除提交"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:276
 msgid "A response was not found for this learner."
-msgstr ""
+msgstr "無法找到此學習者之答案。"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:16
 #, python-format
 msgid ""
 "\n"
 "                            Assessment %(assessment_num)s:\n"
 "                        "
-msgstr ""
+msgstr "\n評分%(assessment_num)s："
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:22
 msgid "Assessment Details"
-msgstr ""
+msgstr "評分詳細資料"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:26
 msgid "Selected Option"
-msgstr ""
+msgstr "選取的評分選項"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:27
 msgid "Feedback"
-msgstr "Phản hồi"
+msgstr "反饋意見"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:29
 msgid "Points Possible"
-msgstr ""
+msgstr "可能的點數"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:18
 msgid "Learn to Assess Responses"
-msgstr "Tìm hiểu để đánh giá phản hồi"
+msgstr " 學習如何評分作答"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:27
 #, python-format
 msgid ""
 "\n"
 "                      In Progress (%(current_progress_num)s of %(training_available_num)s)\n"
 "                  "
@@ -2068,75 +2070,75 @@
 "            <span id=\"oa_step_deadline\" class=\"date ora-datetime\" data-datetime=\"%(due_date)s\" data-string=\"due {date} (in %(time_until)s)\" data-timezone=\"%(user_timezone)s\" data-language=\"%(user_language)s\"></span>\n"
 "            "
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:58
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:66
 msgid "Learning to Assess Responses"
-msgstr ""
+msgstr "學習如何對答案評分"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:61
 msgid ""
 "Before you begin to assess your peers' responses, you'll learn how to "
 "complete peer assessments by reviewing responses that instructors have "
 "already assessed. If you select the same options for the response that the "
 "instructor selected, you'll move to the next step. If you don't select the "
 "same options, you'll review the response and try again."
-msgstr ""
+msgstr "在您開始評分您的同儕之前，您將會透過檢視您的教師已經完成評分的部分，來學習如何評分。如果您選擇了與您的教師相同的答案，則您可移動至下一步。反之若您並未選擇相同的評分選項，您將需再次檢視答案並重新選擇。"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:69
 msgid ""
 "Your assessment differs from the instructor's assessment of this response. "
 "Review the response and consider why the instructor may have assessed it "
 "differently. Then, try the assessment again."
-msgstr ""
+msgstr "您的答案與教師不同。請重新檢視答案並思考為何教師與您有不同的意見，之後再重新評分一次。"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:76
 msgid "The response to the prompt above:"
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:98
 msgid "Selected Options Agree"
-msgstr ""
+msgstr "選擇正確的評分選項"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:101
 msgid "The option you selected is the option that the instructor selected."
-msgstr ""
+msgstr "您選擇了與教師相同的評分選項。"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:105
 msgid "Selected Options Differ"
-msgstr ""
+msgstr "選擇不同的評分選項"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:108
 msgid ""
 "The option you selected is not the option that the instructor selected."
-msgstr ""
+msgstr "您選擇了與教師不同的評分選項。"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:144
 msgid "We could not check your assessment"
-msgstr "Chúng tôi không thể kiểm tra đánh giá của bạn"
+msgstr "我們無法檢查您的作業。"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training.html:151
 msgid "Compare your selections with the instructor's selections"
-msgstr ""
+msgstr "比較您與教師之間的選項"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training_closed.html:29
 msgid ""
 "The due date for this step has passed. This step is now closed. You can no "
 "longer continue with this assignment, and you will receive a grade of "
 "Incomplete."
 msgstr ""
 
 #: openassessment/templates/openassessmentblock/student_training/student_training_error.html:18
 msgid "Error Loading Learner Training Examples"
-msgstr ""
+msgstr "載入評分訓練發生錯誤"
 
 #: openassessment/templates/openassessmentblock/student_training/student_training_error.html:21
 msgid "The Learner Training Step of this assignment could not be loaded."
-msgstr ""
+msgstr "評分訓練步驟的任務無法載入。"
 
 #: openassessment/xblock/data_conversion.py:263
 msgid "You must provide options selected in the assessment."
 msgstr ""
 
 #: openassessment/xblock/data_conversion.py:266
 msgid "You must provide overall feedback in the assessment."
@@ -2148,71 +2150,71 @@
 
 #: openassessment/xblock/grade_mixin.py:77
 #: openassessment/xblock/leaderboard_mixin.py:61
 #: openassessment/xblock/self_assessment_mixin.py:42
 #: openassessment/xblock/student_training_mixin.py:56
 #: openassessment/xblock/student_training_mixin.py:264
 msgid "An unexpected error occurred."
-msgstr "Đã xảy ra lỗi không mong muốn."
+msgstr "ㄧ個未預期的錯誤發生。"
 
 #: openassessment/xblock/grade_mixin.py:175
 msgid "Peer Assessment"
-msgstr "Đánh giá giữa các học viên"
+msgstr "同儕互評"
 
 #: openassessment/xblock/grade_mixin.py:177
 msgid "Self Assessment"
-msgstr "Tự Đánh Giá"
+msgstr "自我評量"
 
 #: openassessment/xblock/grade_mixin.py:217
 msgid "Assessment feedback could not be saved."
-msgstr "Phản hồi đánh giá không được lưu."
+msgstr "無法儲存評分的反饋意見"
 
 #: openassessment/xblock/grade_mixin.py:228
 msgid "Feedback saved."
-msgstr "Phản hồi lưu."
+msgstr "反饋意見已儲存。"
 
 #: openassessment/xblock/grade_mixin.py:362
 #: openassessment/xblock/grade_mixin.py:508
 msgid "Staff Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:368
 msgid "Peer Median Grade"
-msgstr ""
+msgstr "同儕平均分數"
 
 #: openassessment/xblock/grade_mixin.py:373
 #: openassessment/xblock/grade_mixin.py:515
 #, python-brace-format
 msgid "Peer {peer_index}"
-msgstr ""
+msgstr "同儕 {peer_index}"
 
 #: openassessment/xblock/grade_mixin.py:374
 msgid "Peer Comments"
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Self Assessment Grade"
-msgstr ""
+msgstr "自我評量分數"
 
 #: openassessment/xblock/grade_mixin.py:384
 msgid "Your Self Assessment"
-msgstr "Tự đánh giá"
+msgstr "您的自我評分"
 
 #: openassessment/xblock/grade_mixin.py:385
 #: openassessment/xblock/grade_mixin.py:527
 msgid "Your Comments"
-msgstr ""
+msgstr "你的評論"
 
 #: openassessment/xblock/grade_mixin.py:481
 msgid "Waiting for peer reviews"
-msgstr ""
+msgstr "等待同儕觀摩"
 
 #: openassessment/xblock/grade_mixin.py:520
 msgid "Peer"
-msgstr "Bạn học"
+msgstr "同儕"
 
 #: openassessment/xblock/grade_mixin.py:651
 msgid "The grade for this problem is determined by your Staff Grade."
 msgstr ""
 
 #: openassessment/xblock/grade_mixin.py:653
 msgid ""
@@ -2255,35 +2257,35 @@
 
 #: openassessment/xblock/openassesment_template_mixin.py:23
 msgid "Self Assessment to Staff Assessment"
 msgstr ""
 
 #: openassessment/xblock/peer_assessment_mixin.py:61
 msgid "You must submit a response before you can perform a peer assessment."
-msgstr ""
+msgstr "您必須先送出答案才能開始進行同儕互評。"
 
 #: openassessment/xblock/peer_assessment_mixin.py:73
 msgid ""
 "This feedback has already been submitted or the submission has been "
 "cancelled."
-msgstr "Thông tin phản hồi này đã được gửi hoặc việc nộp đã bị hủy."
+msgstr ""
 
 #: openassessment/xblock/peer_assessment_mixin.py:99
 #: openassessment/xblock/peer_assessment_mixin.py:105
 msgid "Your peer assessment could not be submitted."
-msgstr "Phần đánh giá giữa các học viên của bạn không thể được nộp."
+msgstr "無法送出您的同儕評量。"
 
 #: openassessment/xblock/peer_assessment_mixin.py:120
 #: openassessment/xblock/student_training_mixin.py:270
 msgid "Could not update workflow status."
-msgstr "Không thể cập nhật trạng thái công việc."
+msgstr "無法更新工作流程狀態。"
 
 #: openassessment/xblock/peer_assessment_mixin.py:128
 msgid "Could not load peer assessment."
-msgstr "Không thể tải đánh giá giữa các học viên."
+msgstr "無法載入同儕評量。"
 
 #: openassessment/xblock/peer_assessment_mixin.py:215
 msgid "Submit your assessment and review another response"
 msgstr ""
 
 #: openassessment/xblock/peer_assessment_mixin.py:219
 msgid "Submit your assessment and move to next step"
@@ -2295,39 +2297,39 @@
 msgstr ""
 
 #: openassessment/xblock/resolve_dates.py:52
 #, python-brace-format
 msgid ""
 "'{date}' is an invalid date format. Make sure the date is formatted as YYYY-"
 "MM-DDTHH:MM:SS."
-msgstr ""
+msgstr "'{date}'不是一個合法的日期格式，請確定您使用 YYYY-MM-DDTHH:MM:SS 的標準日期格式。"
 
 #: openassessment/xblock/resolve_dates.py:57
 #, python-brace-format
 msgid "'{date}' must be a date string or datetime"
-msgstr ""
+msgstr "'{date}' 必須是個日期字串或是datetime型態"
 
 #: openassessment/xblock/resolve_dates.py:210
 #, python-brace-format
 msgid ""
 "This step's start date '{start}' cannot be earlier than the previous step's "
 "start date '{prev}'."
-msgstr ""
+msgstr "此步驟的起始時間 '{start}' 不能早於前一步驟的起始時間 '{prev}'。"
 
 #: openassessment/xblock/resolve_dates.py:218
 #, python-brace-format
 msgid ""
 "This step's due date '{due}' cannot be later than the next step's due date "
 "'{prev}'."
-msgstr ""
+msgstr "此步驟的截止時間 '{due}' 不能早於前一步驟的截止時間 '{prev}'。"
 
 #: openassessment/xblock/resolve_dates.py:234
 #, python-brace-format
 msgid "The start date '{start}' cannot be later than the due date '{due}'"
-msgstr ""
+msgstr "起始時間 '{start}' 不能晚於截止時間 '{due}'"
 
 #: openassessment/xblock/rubric_reuse_mixin.py:62
 msgid "You must specify a block id from which to copy a rubric."
 msgstr ""
 
 #: openassessment/xblock/rubric_reuse_mixin.py:66
 msgid "Invalid block id."
@@ -2337,28 +2339,28 @@
 #, python-brace-format
 msgid ""
 "No Open Response Assessment found in {course_id} with block id {block_id}"
 msgstr ""
 
 #: openassessment/xblock/self_assessment_mixin.py:142
 msgid "You must submit a response before you can perform a self-assessment."
-msgstr "Bạn phải nộp một phản hồi trước khi bạn có thể thực hiện tự đánh giá."
+msgstr "您必須先送出答案才能開始進行自我評量。"
 
 #: openassessment/xblock/self_assessment_mixin.py:165
 #: openassessment/xblock/self_assessment_mixin.py:173
 msgid "Your self assessment could not be submitted."
-msgstr "Tự đánh giá của bạn không thể được nộp."
+msgstr "無法送出您的自我評量。"
 
 #: openassessment/xblock/staff_area_mixin.py:42
 msgid "You do not have permission to schedule training"
-msgstr "Bạn không có quyền để lên lịch đào tạo"
+msgstr "您沒有權限排序訓練"
 
 #: openassessment/xblock/staff_area_mixin.py:43
 msgid "You do not have permission to reschedule tasks."
-msgstr "Bạn không có quyền để sắp xếp lại các nhiệm vụ."
+msgstr "您沒有權限重新排序任務。"
 
 #: openassessment/xblock/staff_area_mixin.py:69
 msgid "You do not have permission to access the ORA staff area"
 msgstr ""
 
 #: openassessment/xblock/staff_area_mixin.py:70
 msgid "You do not have permission to access ORA learner information."
@@ -2406,15 +2408,15 @@
 
 #: openassessment/xblock/staff_area_mixin.py:382
 msgid "Error getting staff grade ungraded and checked out counts."
 msgstr ""
 
 #: openassessment/xblock/staff_area_mixin.py:672
 msgid "Please enter valid reason to remove the submission."
-msgstr ""
+msgstr "請輸入有效的原因來移除這個提交。"
 
 #: openassessment/xblock/staff_area_mixin.py:683
 msgid "Submission not found"
 msgstr ""
 
 #: openassessment/xblock/staff_area_mixin.py:694
 msgid "Submission for team assignment has no associated team submission"
@@ -2457,40 +2459,40 @@
 msgid ""
 "Check back later to see if a course staff member has assessed your response."
 " You will receive your grade after the assessment is complete."
 msgstr ""
 
 #: openassessment/xblock/staff_assessment_mixin.py:204
 msgid "You Must Complete the Steps Above to View Your Grade"
-msgstr ""
+msgstr "您必須完成以上這些步驟才能查看您的分數"
 
 #: openassessment/xblock/staff_assessment_mixin.py:205
 msgid ""
 "Although a course staff member has assessed your response, you will receive "
 "your grade only after you have completed all the required steps of this "
 "problem."
 msgstr ""
 
 #: openassessment/xblock/student_training_mixin.py:227
 msgid "Missing options_selected key in request"
-msgstr ""
+msgstr "需求中缺少了options_selected的值"
 
 #: openassessment/xblock/student_training_mixin.py:229
 msgid "options_selected must be a dictionary"
-msgstr ""
+msgstr "options_selected 的值必須是個目錄"
 
 #: openassessment/xblock/student_training_mixin.py:254
 #: openassessment/xblock/student_training_mixin.py:259
 msgid "Your scores could not be checked."
-msgstr ""
+msgstr "無法檢查您的分數。"
 
 #: openassessment/xblock/studio_mixin.py:224
 #: openassessment/xblock/studio_mixin.py:236
 msgid "Error updating XBlock configuration"
-msgstr ""
+msgstr "更新XBlock設定的錯誤"
 
 #: openassessment/xblock/studio_mixin.py:241
 msgid "Error: Text Response and File Upload Response cannot both be disabled"
 msgstr ""
 
 #: openassessment/xblock/studio_mixin.py:245
 msgid ""
@@ -2501,31 +2503,31 @@
 msgid ""
 "Error: When File Upload Response is disabled, Text Response must be Required"
 msgstr ""
 
 #: openassessment/xblock/studio_mixin.py:272
 #, python-brace-format
 msgid "Validation error: {error}"
-msgstr "Xác nhận lỗi: {error}"
+msgstr "驗證錯誤：{error}"
 
 #: openassessment/xblock/studio_mixin.py:303
 msgid "Successfully updated OpenAssessment XBlock"
-msgstr ""
+msgstr "成功更新 OpenAssessment XBlock"
 
 #: openassessment/xblock/submission_mixin.py:118
 msgid "\"submission\" required to submit answer."
-msgstr ""
+msgstr "\"submission\"需要提交答案"
 
 #: openassessment/xblock/submission_mixin.py:139
 msgid "To submit a response, view this component in Preview or Live mode."
-msgstr ""
+msgstr "為了送出您的回應，請於 \"預覽\" 或是 \"線上模式\" 檢視此組件。"
 
 #: openassessment/xblock/submission_mixin.py:145
 msgid "Multiple submissions are not allowed."
-msgstr ""
+msgstr "不允許同時多個送出。"
 
 #: openassessment/xblock/submission_mixin.py:178
 msgid "Response exceeds maximum allowed size."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:180
 msgid ""
@@ -2535,140 +2537,140 @@
 
 #: openassessment/xblock/submission_mixin.py:200
 msgid "Submission cannot be empty. Please refresh the page and try again."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
-msgstr ""
+msgstr "API 回應了一個非典型的例外。"
 
 #: openassessment/xblock/submission_mixin.py:261
 msgid "This response could not be saved."
-msgstr "Không thể lưu câu trả lời này."
+msgstr "這個作答無法儲存。"
 
 #: openassessment/xblock/submission_mixin.py:265
 msgid "This response was not submitted."
-msgstr "Phản hồi này đã không được gửi."
+msgstr "這個答案並被未提交。"
 
 #: openassessment/xblock/submission_mixin.py:281
 msgid "Files descriptions were not submitted."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:320
 msgid "Files metadata could not be saved."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:472
 msgid "There was an error uploading your file."
-msgstr ""
+msgstr "在上傳您的檔案時發生了一個錯誤。"
 
 #: openassessment/xblock/submission_mixin.py:484
 msgid "Only a single file upload is allowed for this assessment."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:495
 msgid ""
 "File upload failed: unsupported file type.Only the supported file types can "
 "be uploaded.If you have questions, please reach out to the course team."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:508
 msgid "Error retrieving upload URL."
-msgstr "Lỗi truy xuất URL tải lên."
+msgstr "檢索上傳網址錯誤。"
 
 #: openassessment/xblock/submission_mixin.py:790
 msgid "This response has been saved but not submitted."
-msgstr "Câu trả lời này đã được lưu nhưng chưa được gửi đi."
+msgstr "這一份作答已經儲存了，但仍未提交。"
 
 #: openassessment/xblock/submission_mixin.py:791
 msgid "This response has not been saved."
-msgstr "Câu trả lời này chưa được lưu."
+msgstr "這一個作答還沒有被儲存。"
 
 #: openassessment/xblock/validation.py:118
 msgid "This problem must include at least one assessment."
-msgstr "Vấn đề này phải bao gồm ít nhất một đánh giá."
+msgstr "問題中必須至少包含一個評量。"
 
 #: openassessment/xblock/validation.py:122
 msgid "The assessment order you selected is invalid."
-msgstr "Trình tự đánh giá bạn chọn không hợp lệ."
+msgstr "您選擇的評分順序是無效的。"
 
 #: openassessment/xblock/validation.py:132
 msgid "In peer assessment, the \"Must Grade\" value must be a positive integer."
-msgstr ""
+msgstr "在同儕互評中，\"必需評分數\"的值必須是個正整數。"
 
 #: openassessment/xblock/validation.py:135
 msgid "In peer assessment, the \"Graded By\" value must be a positive integer."
-msgstr "Trong đánh phần giá giữa các học viên, giá trị \"được phân loại bởi \" phải là một số nguyên dương."
+msgstr "在同儕互評中，\"被評分數\"的值必須是個正整數。"
 
 #: openassessment/xblock/validation.py:139
 msgid ""
 "In peer assessment, the \"Must Grade\" value must be greater than or equal "
 "to the \"Graded By\" value."
-msgstr "Trong đánh phần giá giữa các học viên, giá trị của mục \"Phải được phân loại bởi\" phải lớn hơn hoặc bằng với giá trị  của \"được phân loại bởi \"."
+msgstr "在同儕互評中，\"需評分數\"的值必須大於等於\"被評分數\"的值。"
 
 #: openassessment/xblock/validation.py:148
 msgid "You must provide at least one example response for learner training."
-msgstr ""
+msgstr "您必須提供學習者至少一個評分訓練的練習。"
 
 #: openassessment/xblock/validation.py:151
 msgid "Each example response for learner training must be unique."
-msgstr ""
+msgstr "每一個評分練習範例回應一定是唯一的。"
 
 #: openassessment/xblock/validation.py:158
 msgid "The \"required\" value must be true if staff assessment is the only step."
 msgstr ""
 
 #: openassessment/xblock/validation.py:162
 msgid ""
 "The number of assessments cannot be changed after the problem has been "
 "released."
-msgstr ""
+msgstr "問題的評分步驟數量不能再問題釋出後再做修改。"
 
 #: openassessment/xblock/validation.py:167
 msgid ""
 "The assessment type cannot be changed after the problem has been released."
-msgstr ""
+msgstr "問題釋出後您不能再修改評量類別。"
 
 #: openassessment/xblock/validation.py:190
 msgid "This rubric definition is not valid."
-msgstr ""
+msgstr "此評分準則定義並不是有效的。"
 
 #: openassessment/xblock/validation.py:196
 #, python-brace-format
 msgid "Options in '{criterion}' have duplicate name(s): {duplicates}"
-msgstr ""
+msgstr "'{criterion}' 中的評分選項有重複的名稱name(s)：{duplicates}"
 
 #: openassessment/xblock/validation.py:204
 msgid "Criteria with no options must require written feedback."
-msgstr ""
+msgstr "無評分選項之評分標準務必請填寫作答。"
 
 #: openassessment/xblock/validation.py:213
 msgid "Prompts cannot be created or deleted after a problem is released."
-msgstr ""
+msgstr "釋出問題後，題目不能再被建立或刪除。"
 
 #: openassessment/xblock/validation.py:217
 msgid "The number of criteria cannot be changed after a problem is released."
-msgstr ""
+msgstr "問題釋出後您將不能再修改評分標準的數量。"
 
 #: openassessment/xblock/validation.py:230
 msgid "Criteria names cannot be changed after a problem is released"
-msgstr ""
+msgstr "問題釋出後您不能再修改評量標準名稱"
 
 #: openassessment/xblock/validation.py:235
 msgid "The number of options cannot be changed after a problem is released."
-msgstr ""
+msgstr "問題釋出後您將不能再修改選項的數量。"
 
 #: openassessment/xblock/validation.py:240
 msgid "Point values cannot be changed after a problem is released."
-msgstr ""
+msgstr "問題釋出後您不能再修改分數值。"
 
 #: openassessment/xblock/validation.py:291
 msgid "Learner training must have at least one training example."
 msgstr ""
 
 #: openassessment/xblock/validation.py:356
 msgid "Leaderboard number is invalid."
-msgstr ""
+msgstr "排行榜上的數字是無效的。"
 
 #: openassessment/xblock/validation.py:379
 msgid "The submission format is invalid."
-msgstr "Các định dạng cảu bài gửi không hợp lệ."
+msgstr "提交格式是無效的。"
```

### Comparing `ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/vi/LC_MESSAGES/djangojs.po` & `ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,124 +1,128 @@
 # #-#-#-#-#  djangojs.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
-# 7b361a451bd8feeed2dbd9245f836232_a786ad5 <aefa5f09660e622131eca858f9656914_301034>, 2015
-# Hoà Lê Thanh <hoa.lethanh@gmail.com>, 2017
-# NGUYEN CONG NAM <congnam0409@gmail.com>, 2014
-# Nguyen Don Binh <donbinhvn@gmail.com>, 2014
-# NGUYEN HOANG AN <neyugn2909@gmail.com>, 2014
-# Nguyen Nhat Quang <technicalmanager@gmail.com>, 2016
-# Theodora. Tôn Nữ Quý Thiện <thien.tonnu1001@gmail.com>, 2015
-# Le Minh Tri <trilm@hihexa.com>, 2020
-# Trung V. Nguyen <trung.ngvan@gmail.com>, 2015
+# abby li <yc.li@eliteu.cn>, 2019
+# Hu Tong <buildmindht@outlook.com>, 2014
+# Changyue Wang <peterwang.dut@gmail.com>, 2014
+# Dwi Sulfahnur <dwisulfahnur@gmail.com>, 2018
+# Haiyu Zhen <jennifer.zhy@hotmail.com>, 2015
+# ifLab <webmaster@iflab.org>, 2018
+# jg Ma <jg20040308@126.com>, 2016
+# Jiazhen Tan <jessie12@live.cn>, 2016
+# jsgang <jsgang9@gmail.com>, 2015,2017,2021
+# louyihua <supermouselyh@hotmail.com>, 2014
+# Yue Fang <yfang@juilliard.edu>, 2016
+# zhouxuan <lion19930924@163.com>, 2015
+# 张太红 <zth@xjau.edu.cn>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Le Minh Tri <trilm@hihexa.com>, 2020\n"
-"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
+"Last-Translator: jsgang <jsgang9@gmail.com>, 2015,2017,2021\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/edx-platform/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: vi\n"
+"Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:77
 #: openassessment/xblock/static/js/src/oa_server.js:113
 #: openassessment/xblock/static/js/src/oa_server.js:137
 msgid "This section could not be loaded."
-msgstr "Không thể tải mục này."
+msgstr "这个部分无法加载。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:158
 msgid "The staff assessment form could not be loaded."
-msgstr ""
+msgstr "工作人员评测表格无法加载。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:180
 msgid "The display of ungraded and checked out responses could not be loaded."
-msgstr ""
+msgstr "未打分及已通过回答的窗口无法加载。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:214
 msgid "This response could not be submitted."
-msgstr "Không thể gửi câu trả lời này."
+msgstr "该答案无法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:237
 msgid "This response could not be saved."
-msgstr "Không thể lưu câu trả lời này."
+msgstr "该答案无法保存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:262
 msgid "This feedback could not be submitted."
-msgstr "Không thể gửi phản hồi này."
+msgstr "这条反馈无法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:287
 #: openassessment/xblock/static/js/src/oa_server.js:378
 #: openassessment/xblock/static/js/src/oa_server.js:401
 msgid "This assessment could not be submitted."
-msgstr "Không thể gửi đánh giá này."
+msgstr "这份评测无法提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:424
 msgid "One or more rescheduling tasks failed."
-msgstr "Một hoặc nhiều tác vụ điều chỉnh lịch học đã thất bại."
+msgstr "一项或几项改期任务失败了。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:483
 msgid "This problem could not be saved."
-msgstr "Không thể lưu câu hỏi này."
+msgstr "该问题无法保存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:504
 msgid "The server could not be contacted."
-msgstr "Không thể liên hệ với máy chủ."
+msgstr "无法联系服务器。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:530
 msgid "Could not retrieve upload url."
-msgstr "Không thể tìm thấy đường dẫn tải lên."
+msgstr "不能读取上传链接地址"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:549
 #: openassessment/xblock/static/js/src/oa_server.js:568
 msgid "Server error."
-msgstr ""
+msgstr "服务器错误。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:588
 msgid "Could not retrieve download url."
-msgstr "Không thể tìm thấy đường dẫn tải xuống."
+msgstr "不能读取下载链接地址"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:614
 msgid "The submission could not be removed from the grading pool."
-msgstr "Bài nộp không thể gỡ bỏ khỏi hệ thống chấm điểm."
+msgstr "该提交无法从评分池中删除。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:670
 msgid "Multiple teams returned for course"
 msgstr ""
 
@@ -155,98 +159,98 @@
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
-msgstr ""
+msgstr "单元名"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:98
 msgid "Units"
-msgstr ""
+msgstr "单元"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:105
 msgid "Assessment"
-msgstr ""
+msgstr "评分"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:106
 msgid "Assessments"
-msgstr ""
+msgstr "评分"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:113
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:114
 msgid "Total Responses"
-msgstr ""
+msgstr "解答总数"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:121
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:122
 msgid "Training"
-msgstr ""
+msgstr "训练"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:129
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:130
 msgid "Peer"
-msgstr ""
+msgstr "同行"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:137
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:138
 msgid "Self"
-msgstr ""
+msgstr "自己"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:145
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:146
 msgid "Waiting"
-msgstr ""
+msgstr "等待"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:153
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:154
 msgid "Staff"
-msgstr ""
+msgstr "工作人员"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:161
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
-msgstr ""
+msgstr "最终收获得分"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
-msgstr ""
+msgstr "开放评估列表不可用"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:302
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:353
 msgid "Please wait"
-msgstr ""
+msgstr "请稍候"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:326
 msgid "Block view is unavailable"
-msgstr ""
+msgstr "块视图不可用"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
-msgstr ""
+msgstr "返回完整列表"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -258,54 +262,54 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
-msgstr "Trạng Thái Trả Lời Của Bạn"
+msgstr "您的答案的状态"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:429
 msgid "This response has not been saved."
-msgstr "Câu trả lời này chưa được lưu."
+msgstr "该答案还没有被保存。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:434
 msgid ""
 "If you leave this page without saving or submitting your response, you will "
 "lose any work you have done on the response."
-msgstr ""
+msgstr "如果您不保存或者提交答案就离开，您可能会丢失掉写完的一切。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:452
 msgid "Saving..."
-msgstr "Đang lưu..."
+msgstr "正在保存…"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:472
 msgid "This response has been saved but not submitted."
-msgstr "Câu trả lời này đã được lưu nhưng chưa được gửi đi."
+msgstr "该答案已经保存了，但仍未提交。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
-msgstr "Lỗi"
+msgstr "错误"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
-msgstr "Bạn sắp nộp câu trả lời cho bài tập này. Sau khi gửi bài bạn sẽ không thể chỉnh sửa hoặc nộp bài mới. "
+msgstr "您将会提交对本次作业的答案。提交后，您将无法修改或者提交新的答案。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:576
 msgid "Individual file size must be {max_files_mb}MB or less."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -320,25 +324,25 @@
 msgid "The maximum number files that can be saved is "
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 #: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
-msgstr ""
+msgstr "描述"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 msgid "(required):"
-msgstr ""
+msgstr "(必须):"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
-msgstr ""
+msgstr "缩略视图"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -349,26 +353,26 @@
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_self.js:138
 msgid ""
 "If you leave this page without submitting your self assessment, you will "
 "lose any work you have done."
-msgstr ""
+msgstr "如果您未提交您的自我评估就离开此页面，您将丢失所做的一切。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:143
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:253
 msgid "Unexpected server error."
-msgstr ""
+msgstr "服务器异常错误。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:147
 msgid "You must provide a learner name."
-msgstr ""
+msgstr "您必须提供一个学生姓名。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:214
 msgid ""
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
 msgstr ""
@@ -377,34 +381,34 @@
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
-msgstr ""
+msgstr "获取未评分回复数量出现错误"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:538
 msgid ""
 "If you leave this page without submitting your staff assessment, you will "
 "lose any work you have done."
-msgstr ""
+msgstr "如果您未提交您的员工评估就离开此页面，您将丢失所做的一切。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_training.js:130
 msgid "Feedback available for selection."
-msgstr ""
+msgstr "可供选择的反馈。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_peer.js:217
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
-msgstr ""
+msgstr "如果您离开本页时没有提交您的同学互评，您将丢失您所做的一切。"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
@@ -451,128 +455,128 @@
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
-msgstr ""
+msgstr "不能加载"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Paragraph"
-msgstr ""
+msgstr "段落"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Preformatted"
-msgstr ""
+msgstr "格式化"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 3"
-msgstr ""
+msgstr "标题 3"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 4"
-msgstr ""
+msgstr "标题 4"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 5"
-msgstr ""
+msgstr "标题 5"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_tiny_mce.js:66
 msgid "Heading 6"
-msgstr ""
+msgstr "标题 6"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:43
 msgid "Unnamed Option"
-msgstr "Tùy Chọn Chưa Đặt Tên"
+msgstr "未命名选项"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
-msgstr "Không Được Chọn"
+msgstr "未选中"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
-msgstr ""
+msgstr "标准已添加"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
-msgstr "Đã Xóa Tùy Chọn"
+msgstr "选项已删除"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:152
 msgid ""
 "You have deleted an option. That option has been removed from its criterion "
 "in the sample responses in the Learner Training step. You might have to "
 "select a new option for the criterion."
-msgstr ""
+msgstr "您已删除一个选项。此选项已从“学员训练”步骤中的回复示例标准中删除。您可能必须为此标准选择一个新选项。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:188
 msgid ""
 "You have deleted all the options for this criterion. The criterion has been "
 "removed from the sample responses in the Learner Training step."
-msgstr ""
+msgstr "您已删除此标准的所有选项。此标准已从“学员训练”步骤的回复示例中删除。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:214
 msgid "Criterion Deleted"
-msgstr ""
+msgstr "规范已删除"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:216
 msgid ""
 "You have deleted a criterion. The criterion has been removed from the "
 "example responses in the Learner Training step."
-msgstr ""
+msgstr "您已删除了一个标准。此标准已从“学员训练”步骤的回复示例中撤销。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:394
 msgid "Warning"
-msgstr "Cảnh báo"
+msgstr "警告"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:395
 msgid ""
 "Changes to steps that are not selected as part of the assignment will not be"
 " saved."
-msgstr "Những thay đổi ở các bước không được chọn thuộc một phần của bài tập sẽ không được lưu."
+msgstr "未作为作业部分的步骤变更将不会被保存。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:91
 msgid "File types can not be empty."
-msgstr ""
+msgstr "文件类型不能为空。"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
-msgstr ""
+msgstr "下列文件类型不可用："
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
 msgstr ""
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
```

### Comparing `ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/django.po` & `ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/django.mo` & `ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo` & `ora2-5.1.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/management/commands/collect_ora2_data.py` & `ora2-5.1.0/openassessment/management/commands/collect_ora2_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/management/commands/create_oa_submissions.py` & `ora2-5.1.0/openassessment/management/commands/create_oa_submissions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/management/commands/create_oa_submissions_from_file.py` & `ora2-5.1.0/openassessment/management/commands/create_oa_submissions_from_file.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/management/commands/upload_oa_data.py` & `ora2-5.1.0/openassessment/management/commands/upload_oa_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/runtime_imports/classes.py` & `ora2-5.1.0/openassessment/runtime_imports/classes.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/runtime_imports/functions.py` & `ora2-5.1.0/openassessment/runtime_imports/functions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/admin.py` & `ora2-5.1.0/openassessment/staffgrader/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/migrations/0001_initial.py` & `ora2-5.1.0/openassessment/staffgrader/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/models/submission_lock.py` & `ora2-5.1.0/openassessment/staffgrader/models/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/serializers/assessments.py` & `ora2-5.1.0/openassessment/staffgrader/serializers/assessments.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/serializers/submission_list.py` & `ora2-5.1.0/openassessment/staffgrader/serializers/submission_list.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/serializers/submission_lock.py` & `ora2-5.1.0/openassessment/staffgrader/serializers/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/staffgrader/staff_grader_mixin.py` & `ora2-5.1.0/openassessment/staffgrader/staff_grader_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_option.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_training_example.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_closed.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_complete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_no_team.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/message/oa_message_open.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/message/oa_message_open.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_base.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_base.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_latex_preview.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_latex_preview.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_rubric.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_submission_answer.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_submission_answer.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 {% spaceless %}
 {% load i18n %}
 
 {% if file_upload_type %}
   <div class="{{ class_prefix }}__display__file {% if not team_file_urls %}is--hidden{% endif %} submission__{{ file_upload_type }}__upload" data-upload-type="{{ file_upload_type }}">
         {% if team_file_urls %}
+        <hr/>
         <h5 class="submission__answer__part__text__title">
           {% trans "Files that were uploaded by your teammates:" %}
         </h5>
         {% endif %}
 
         <div class="submission__answer__files">
         {% for file in team_file_urls %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% spaceless %} {% load i18n %} {% if file_upload_type %}
 {% if team_file_urls %}
+===============================================================================
 ** {% trans "Files that were uploaded by your teammates:" %} **
 {% endif %}
 {% for file in team_file_urls %}
 % if not file.download_url %} deleted {% endif %}> {% if file.download_url %}
 {% if file_upload_type == "image" %} {% if file.description %}
 {{ file.description }}:
 {% endif %}
```

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/oa_uploaded_file.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,50 +62,50 @@
         <div class="wrapper--step__content">
             <div class="step__instruction">
                 <p>
                   {% if team_name %}
                     {% trans "Enter your team's response to the prompt." %}
                     {% if submission_due %}
                       {% blocktrans %}
-                        You can save your progress and return to complete your team's response at any time before the due date
+                        Your work will save automatically and you can return to complete your team's response at any time before the due date
                       {% endblocktrans %}
                       (<span class="step__deadline">
                         <span id="oa_step_deadline_response"
                           class="date ora-datetime"
                           data-datetime="{{ submission_due|timezone:'UTC'|date:'c' }}"
                           data-timezone="{{ user_timezone }}"
                           data-format="longDateTime"
                           data-language="{{ user_language }}">
                         </span>
                       </span>).
                     {% else %}
                       {% blocktrans %}
-                        You can save your progress and return to complete your team's response at any time.
+                        Your work will save automatically and you can return to complete your team's response at any time.
                       {% endblocktrans %}
                     {% endif %}
                     <strong class="emphasis">
-                      {% trans "After you submit a response on behalf of your team, it cannot be edited" %}
-                    </strong>.
+                      {% trans "After you submit a response on behalf of your team, it cannot be edited." %}
+                    </strong>
                   {% else %}
                     {% trans "Enter your response to the prompt." %}
                     {% if submission_due %}
                       {% blocktrans %}
-                        You can save your progress and return to complete your response at any time before the due date
+                        Your work will save automatically and you can return to complete your response at any time before the due date
                       {% endblocktrans %}
                       (<span class="step__deadline">
                           <span id="oa_step_deadline_response"
                             class="date ora-datetime"
                             data-datetime="{{ submission_due|timezone:'UTC'|date:'c' }}"
                             data-timezone="{{ user_timezone }}"
                             data-format="longDateTime"
                             data-language="{{ user_language }}">
                           </span>
                       </span>).
                     {% else %}
-                      {% trans "You can save your progress and return to complete your response at any time." %}
+                      {% trans "Your work will save automatically and you can return to complete your response at any time." %}
                     {% endif %}
                     <strong class="emphasis">{% trans "After you submit your response, you cannot edit it" %}</strong>.
                   {% endif %}
                 </p>
             </div>
             {% if show_rubric_during_response %}
                 <div class="step__rubric">
@@ -186,15 +186,14 @@
                                         {% endif %}
                                     </div>
                                     <textarea
                                         id="submission__answer__part__text__{{ forloop.counter }}__{{ xblock_id }}"
                                         class="submission__answer__part__text__value"
                                         data-preview="submission__{{ forloop.counter }}"
                                         aria-labelledby="submission__answer__part__text__title__{{ forloop.counter }}__{{ xblock_id }}"
-                                        aria-describedby="submission__answer__tip__{{ xblock_id }}"
                                         placeholder="{% trans "Enter your response to the prompt above." %}"
                                         maxlength="100000"
                                     >{{ part.text }}</textarea>
                                 </div>
                                 {% with forloop.counter|stringformat:"s" as submission_num %}
                                     {% include "openassessmentblock/oa_latex_preview.html" with id="submission__"|add:xblock_id|add:submission_num elem="div" preview_name="submission__"|add:submission_num %}
                                 {% endwith %}
@@ -220,27 +219,27 @@
                                   <div class="message message--inline message--error message--error-server" tabindex="-1">
                                       <h5 class="message__title">{% trans "We could not save your progress" %}</h5>
                                       <div class="message__content"></div>
                                   </div>
 
                                   <ul class="list list--actions">
                                       <li class="list--actions__item">
-                                          <button type="submit" class="action action--save submission__save" aria-describedby="response__save_status__{{ xblock_id }}" disabled>
-                                              {% trans "Save your progress" %}
-                                          </button>
-
-                                          <div id="response__save_status__{{ xblock_id }}" class="save__submission__label response__submission__label">
-                                              <span class="sr">{% trans "Your Submission Status" %}:</span>
-                                              {{ save_status }}
+                                          <div id="response__save_status__{{ xblock_id }}" class="response__submission__label">
+                                              <span class="save__submission__icon icon fa fa-circle-o" aria-hidden="true"></span>
+                                              <span class="sr">{% trans "Status of Your Response" %}:</span>
+                                              <span class="save__submission__label">{{ save_status }}</span>
                                           </div>
                                       </li>
                                   </ul>
                               </div>
                           </li>
                           {% endif %}
+                          {% if text_response and file_upload_type %}
+                            <hr/>
+                          {% endif %}
                           {% if file_upload_type %}
                             <h5 class="submission__upload__files__title">
                               {% trans "File Uploads " %}
                               {% if file_upload_response == "required" %}
                                 {% trans "(Required)" %}
                               {% elif file_upload_response == "optional" %}
                                 {% trans "(Optional)" %}
@@ -269,40 +268,35 @@
                                 <label class="sr" for="submission_answer_upload_{{ xblock_id }}">
                                   {% if allow_multiple_files %}
                                       {% trans "Select one or more files to upload for this submission." %}
                                   {% else %}
                                       {% trans "Select a file to upload for this submission." %}
                                   {% endif %}
                                 </label>
-                                <input type="file" class="submission__answer__upload file--upload" id="submission_answer_upload_{{ xblock_id }}" {% if allow_multiple_files %}multiple=""{% endif %} accept="{{white_listed_file_types|join:", "}}">
-                                <span>
+                                <div>
                                   {% trans "Supported file types: " %}{{ white_listed_file_types|join:", "}}
-                                </span>
+                                </div>
+                                <input type="file" class="submission__answer__upload file--upload" id="submission_answer_upload_{{ xblock_id }}" {% if allow_multiple_files %}multiple=""{% endif %} accept="{{white_listed_file_types|join:", "}}">
                                 <button type="submit" class="file__upload action action--upload" disabled>
                                   {% if allow_multiple_files %}
                                       {% trans "Upload files" %}
                                   {% else %}
                                       {% trans "Upload file" %}
                                   {% endif %}
                                 </button>
                                 <div class="files__descriptions"></div>
                             </li>
                           {% endif %}
                           <li class="field">
                           {% include "openassessmentblock/oa_uploaded_file.html" with file_upload_type=file_upload_type file_urls=file_urls class_prefix="submission__answer" including_template="response" xblock_id=xblock_id %}
                           </li>
-                          <hr/>
                           <li class="field">
-                          {% include "openassessmentblock/oa_team_uploaded_files.html" with file_upload_type=file_upload_type team_file_urls=team_file_urls class_prefix="submission__team__answer" including_template="response" xblock_id=xblock_id %}
+                            {% include "openassessmentblock/oa_team_uploaded_files.html" with file_upload_type=file_upload_type team_file_urls=team_file_urls class_prefix="submission__team__answer" including_template="response" xblock_id=xblock_id %}
                           </li>
                       </ol>
-
-                      {% if not team_name %}
-                          <span class="tip" id="submission__answer__tip__{{ xblock_id }}">{% trans "You may continue to work on your response until you submit it." %}</span>
-                      {% endif %}
                   </form>
               </div>
               {% if team_name %}
                 <div id='team_concurrency_notice'>
                   {% trans "This is a team submission." %}
                   {% if file_upload_type and text_response %}
                       {% trans "One team member should submit a response with the team’s shared files and a text response on behalf of the entire team." %}
```

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_closed.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_graded.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_submitted.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_closed.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_complete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_closed.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_complete.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_error.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html` & `ora2-5.1.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/templatetags/oa_extras.py` & `ora2-5.1.0/openassessment/templatetags/oa_extras.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/test_utils.py` & `ora2-5.1.0/openassessment/test_utils.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/admin.py` & `ora2-5.1.0/openassessment/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/api.py` & `ora2-5.1.0/openassessment/workflow/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/errors.py` & `ora2-5.1.0/openassessment/workflow/errors.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/migrations/0001_initial.py` & `ora2-5.1.0/openassessment/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/migrations/0003_TeamWorkflows.py` & `ora2-5.1.0/openassessment/workflow/migrations/0003_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/models.py` & `ora2-5.1.0/openassessment/workflow/models.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/serializers.py` & `ora2-5.1.0/openassessment/workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/workflow/team_api.py` & `ora2-5.1.0/openassessment/workflow/team_api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/config_mixin.py` & `ora2-5.1.0/openassessment/xblock/config_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/course_items_listing_mixin.py` & `ora2-5.1.0/openassessment/xblock/course_items_listing_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/data_conversion.py` & `ora2-5.1.0/openassessment/xblock/data_conversion.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/defaults.py` & `ora2-5.1.0/openassessment/xblock/defaults.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/editor_config.py` & `ora2-5.1.0/openassessment/xblock/editor_config.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/grade_mixin.py` & `ora2-5.1.0/openassessment/xblock/grade_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/leaderboard_mixin.py` & `ora2-5.1.0/openassessment/xblock/leaderboard_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/lms_mixin.py` & `ora2-5.1.0/openassessment/xblock/lms_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/load_static.py` & `ora2-5.1.0/openassessment/xblock/load_static.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/message_mixin.py` & `ora2-5.1.0/openassessment/xblock/message_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/mobile.py` & `ora2-5.1.0/openassessment/xblock/mobile.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/openassesment_template_mixin.py` & `ora2-5.1.0/openassessment/xblock/openassesment_template_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/openassessmentblock.py` & `ora2-5.1.0/openassessment/xblock/openassessmentblock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/peer_assessment_mixin.py` & `ora2-5.1.0/openassessment/xblock/peer_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/resolve_dates.py` & `ora2-5.1.0/openassessment/xblock/resolve_dates.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/rubric_reuse_mixin.py` & `ora2-5.1.0/openassessment/xblock/rubric_reuse_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/schema.py` & `ora2-5.1.0/openassessment/xblock/schema.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/self_assessment_mixin.py` & `ora2-5.1.0/openassessment/xblock/self_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/staff_area_mixin.py` & `ora2-5.1.0/openassessment/xblock/staff_area_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/staff_assessment_mixin.py` & `ora2-5.1.0/openassessment/xblock/staff_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/css/lib/backgrid/backgrid.css` & `ora2-5.1.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css` & `ora2-5.1.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/manifest.json` & `ora2-5.1.0/openassessment/xblock/static/dist/manifest.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65%*

 * *Differences: {"'openassessment-lms.css'": "'/openassessment-lms.967dad15c001a5dc6a5e.css'",*

 * * "'openassessment-lms.css.map'": "'/openassessment-lms.967dad15c001a5dc6a5e.css.map'",*

 * * "'openassessment-lms.js'": "'/openassessment-lms.967dad15c001a5dc6a5e.js'",*

 * * "'openassessment-lms.js.map'": "'/openassessment-lms.967dad15c001a5dc6a5e.js.map'",*

 * * "'openassessment-ltr.css'": "'/openassessment-ltr.b9eeb00dfc7524a80658.css'",*

 * * "'openassessment-ltr.css.map'": "'/openassessment-ltr.b9eeb00dfc7524a80658.css.map'",*

 * * "'openassessment- […]*

```diff
@@ -1,22 +1,22 @@
 {
     "base_url": "/static/dist",
     "default-avatar.svg": "/95ec738c0b7faac5b5c9126794446bbd.svg",
     "openassessment-editor-textarea.js": "/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js",
     "openassessment-editor-textarea.js.map": "/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js.map",
     "openassessment-editor-tinymce.js": "/openassessment-editor-tinymce.2cc0cab55c3be729265e.js",
     "openassessment-editor-tinymce.js.map": "/openassessment-editor-tinymce.2cc0cab55c3be729265e.js.map",
-    "openassessment-lms.css": "/openassessment-lms.e009f195cfd3e23b44e3.css",
-    "openassessment-lms.css.map": "/openassessment-lms.e009f195cfd3e23b44e3.css.map",
-    "openassessment-lms.js": "/openassessment-lms.e009f195cfd3e23b44e3.js",
-    "openassessment-lms.js.map": "/openassessment-lms.e009f195cfd3e23b44e3.js.map",
-    "openassessment-ltr.css": "/openassessment-ltr.af4f203c872dac1a24b5.css",
-    "openassessment-ltr.css.map": "/openassessment-ltr.af4f203c872dac1a24b5.css.map",
-    "openassessment-ltr.js": "/openassessment-ltr.af4f203c872dac1a24b5.js",
-    "openassessment-ltr.js.map": "/openassessment-ltr.af4f203c872dac1a24b5.js.map",
-    "openassessment-rtl.css": "/openassessment-rtl.b8d173da7a201af6385c.css",
-    "openassessment-rtl.css.map": "/openassessment-rtl.b8d173da7a201af6385c.css.map",
-    "openassessment-rtl.js": "/openassessment-rtl.b8d173da7a201af6385c.js",
-    "openassessment-rtl.js.map": "/openassessment-rtl.b8d173da7a201af6385c.js.map",
-    "openassessment-studio.js": "/openassessment-studio.1ef78b4390a9cfa2e9b1.js",
-    "openassessment-studio.js.map": "/openassessment-studio.1ef78b4390a9cfa2e9b1.js.map"
+    "openassessment-lms.css": "/openassessment-lms.967dad15c001a5dc6a5e.css",
+    "openassessment-lms.css.map": "/openassessment-lms.967dad15c001a5dc6a5e.css.map",
+    "openassessment-lms.js": "/openassessment-lms.967dad15c001a5dc6a5e.js",
+    "openassessment-lms.js.map": "/openassessment-lms.967dad15c001a5dc6a5e.js.map",
+    "openassessment-ltr.css": "/openassessment-ltr.b9eeb00dfc7524a80658.css",
+    "openassessment-ltr.css.map": "/openassessment-ltr.b9eeb00dfc7524a80658.css.map",
+    "openassessment-ltr.js": "/openassessment-ltr.b9eeb00dfc7524a80658.js",
+    "openassessment-ltr.js.map": "/openassessment-ltr.b9eeb00dfc7524a80658.js.map",
+    "openassessment-rtl.css": "/openassessment-rtl.ef543a27286a069bd958.css",
+    "openassessment-rtl.css.map": "/openassessment-rtl.ef543a27286a069bd958.css.map",
+    "openassessment-rtl.js": "/openassessment-rtl.ef543a27286a069bd958.js",
+    "openassessment-rtl.js.map": "/openassessment-rtl.ef543a27286a069bd958.js.map",
+    "openassessment-studio.js": "/openassessment-studio.13c817d25360969539ff.js",
+    "openassessment-studio.js.map": "/openassessment-studio.13c817d25360969539ff.js.map"
 }
```

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-textarea.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-editor-tinymce.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-lms.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-lms.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.css` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-ltr.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-ltr.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.css` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-rtl.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-rtl.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/dist/openassessment-studio.js` & `ora2-5.1.0/openassessment/xblock/static/dist/openassessment-studio.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/lib/backgrid/backgrid.js` & `ora2-5.1.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js` & `ora2-5.1.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_base.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_base.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_datefactory.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_file_upload.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_grade.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_grade.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_leaderboard.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_message.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_message.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_peer.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_peer.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_prompts.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_response.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_response.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -17,24 +17,30 @@
  * */
 export class ResponseView {
     // Milliseconds between checks for whether we should autosave.
     AUTO_SAVE_POLL_INTERVAL = 2000;
 
     // Required delay after the user changes a response or a save occurs
     // before we can autosave.
-    AUTO_SAVE_WAIT = 30000;
+    AUTO_SAVE_WAIT = 2000;
 
     // Maximum size (500 * 2^20 bytes, approx. 500MB) of a single uploaded file.
     MAX_FILE_SIZE = 500 * (1024 ** 2);
 
     // For user-facing upload limit text.
     MAX_FILES_MB = 500;
 
     UNSAVED_WARNING_KEY = 'learner-response';
 
+    ICON_SAVED = 'fa-check-circle-o';
+
+    ICON_SAVING = 'fa-refresh';
+
+    ICON_ERROR = 'fa-exclamation-circle';
+
     constructor(element, server, fileUploader, responseEditorLoader, baseView, data) {
         this.element = element;
         this.server = server;
         this.fileUploader = fileUploader;
         this.responseEditorLoader = responseEditorLoader;
         this.baseView = baseView;
         this.savedResponse = [];
@@ -270,36 +276,14 @@
      >> true
      * */
     submitEnabled(enabled) {
         return this.baseView.buttonEnabled('.step--response__submit', enabled);
     }
 
     /**
-     Enable/disable the save button.
-     Check whether the save button is enabled.
-
-     Also enables/disables a beforeunload handler to warn
-     users about navigating away from the page with unsaved changes.
-
-     Args:
-     enabled (bool): If specified, set the state of the button.
-
-     Returns:
-     bool: Whether the button is enabled.
-
-     Examples:
-     >> view.saveEnabled(true);  // enable the button
-     >> view.saveEnabled();  // check whether the button is enabled
-     >> true
-     * */
-    saveEnabled(enabled) {
-        return this.baseView.buttonEnabled('.submission__save', enabled);
-    }
-
-    /**
      * Enable/disable the upload button or check whether the upload button is enabled
      *
      * @param {boolean]} enabled - optional param to enable/disable button
      * @returns {boolean} whether the upload button is enabled or not
      *
      * @example
      *     view.uploadEnabled(true);  // enable the upload button
@@ -307,17 +291,27 @@
      */
     uploadEnabled(enabled) {
         return this.baseView.buttonEnabled('.file__upload', enabled);
     }
 
     /**
      Enable/disable the preview button.
+     Check whether the preview button is enabled.
 
-     Works exactly the same way as saveEnabled method.
-     * */
+     Args:
+     enabled (bool): If specified, set the state of the button.
+
+     Returns:
+     bool: Whether the button is enabled.
+
+     Examples:
+     >> view.previewEnabled(true);  // enable the button
+     >> view.previewEnabled();  // check whether the button is enabled
+     >> true
+    */
     previewEnabled(enabled) {
         return this.baseView.buttonEnabled('.submission__preview', enabled);
     }
 
     /**
       Check if there is a file selected but not uploaded yet
       Returns:
@@ -349,28 +343,36 @@
 
     /**
      Set the save status message.
      Retrieve the save status message.
 
      Args:
      msg (string): If specified, the message to display.
+     iconClass (str): If specified, icon to display with save status.
 
      Returns:
      string: The current status message.
      * */
-    /* eslint-disable-next-line consistent-return */
-    saveStatus(msg) {
-        const sel = $('.save__submission__label', this.element);
+    saveStatus(msg, iconClass) {
+        // Create save status text
+        const saveStatusSel = $('.save__submission__label', this.element);
         if (typeof msg === 'undefined') {
-            return sel.text();
+            return saveStatusSel.text();
         }
-        // Setting the HTML will overwrite the screen reader tag,
-        // so prepend it to the message.
-        const label = gettext('Status of Your Response');
-        sel.html(`<span class="sr">${_.escape(label)}:</span>\n${msg}`);
+        saveStatusSel.text(_.escape(msg));
+
+        // Update save status icon, if provided
+        const iconSel = $('.save__submission__icon', this.element);
+        let iconClasses = 'save__submission__icon icon fa ';
+        if (typeof msg === 'string') {
+            iconClasses += _.escape(iconClass);
+        }
+        iconSel.attr('class', iconClasses);
+
+        return saveStatusSel.text();
     }
 
     /**
      Set the response texts.
      Retrieve the response texts.
 
      Args:
@@ -406,17 +408,15 @@
     autoSave() {
         const timeSinceLastChange = Date.now() - this.lastChangeTime;
 
         // We only autosave if the following conditions are met:
         // (1) The response has changed.  We don't need to keep saving the same response.
         // (2) Sufficient time has passed since the user last made a change to the response.
         //      We don't want to save a response while the user is in the middle of typing.
-        // (3) No errors occurred on the last save.  We don't want to keep refreshing
-        //      the error message in the UI.  (The user can still retry the save manually).
-        if (this.responseChanged() && timeSinceLastChange > this.AUTO_SAVE_WAIT && !this.errorOnLastSave) {
+        if (this.responseChanged() && timeSinceLastChange > this.AUTO_SAVE_WAIT) {
             this.save();
         }
     }
 
     /**
      Enable/disable the submission and save buttons based on whether
      the user has entered a response.
@@ -424,17 +424,21 @@
     handleResponseChanged() {
         this.checkSubmissionAbility();
 
         // Update the save button, save status, and "unsaved changes" warning
         // only if the response has changed
         if (this.responseChanged()) {
             const saveAbility = this.checkSaveAbility();
-            this.saveEnabled(saveAbility);
             this.previewEnabled(saveAbility);
-            this.saveStatus(gettext('This response has not been saved.'));
+
+            // If there was an error, preserve error status
+            if (!this.errorOnLastSave) {
+                this.saveStatus(gettext('Saving draft'), this.ICON_SAVING);
+            }
+
             this.baseView.unsavedWarningEnabled(
                 true,
                 this.UNSAVED_WARNING_KEY,
                 // eslint-disable-next-line max-len
                 gettext('If you leave this page without saving or submitting your response, you will lose any work you have done on the response.'),
             );
         }
@@ -443,47 +447,53 @@
         this.lastChangeTime = Date.now();
     }
 
     /**
      Save a response without submitting it.
      * */
     save() {
-        // If there were errors on previous calls to save, forget
-        // about them for now.  If an error occurs on *this* save,
-        // we'll set this back to true in the error handler.
-        this.errorOnLastSave = false;
-
         // Update the save status and error notifications
-        this.saveStatus(gettext('Saving...'));
-        this.baseView.toggleActionError('save', null);
+        // ... unless there was an error, this helps avoid unnecessary UI refreshes.
+        if (!this.errorOnLastSave) {
+            this.saveStatus(gettext('Saving draft...'), this.ICON_SAVING);
+        }
 
         // Disable the "unsaved changes" warning
         this.baseView.unsavedWarningEnabled(false, this.UNSAVED_WARNING_KEY);
 
         const view = this;
         const savedResponse = this.response();
+
         this.server.save(savedResponse).done(() => {
             // Remember which response we saved, once the server confirms that it's been saved...
             view.savedResponse = savedResponse;
 
             // ... but update the UI based on what the user may have entered
             // since hitting the save button.
             view.checkSubmissionAbility();
 
             const currentResponse = view.response();
             const currentResponseEqualsSaved = currentResponse.every((element, index) => element === savedResponse[index]);
             if (currentResponseEqualsSaved) {
-                view.saveEnabled(false);
-                const msg = gettext('This response has been saved but not submitted.');
-                view.saveStatus(msg);
+                const msg = gettext('Draft saved!');
+                view.saveStatus(msg, this.ICON_SAVED);
                 view.baseView.srReadTexts([msg]);
+
+                // Disable error
+                this.baseView.toggleActionError('save', null);
+                view.errorOnLastSave = false;
             }
         }).fail((errMsg) => {
-            view.saveStatus(gettext('Error'));
-            view.baseView.toggleActionError('save', errMsg);
+            // Debounce error banner, this won't capture new errors, but will keep
+            // us from defocusing text area, allowing user to continue to edit their
+            // response.
+            if (!view.errorOnLastSave) {
+                view.saveStatus(gettext('Error'), this.ICON_ERROR);
+                view.baseView.toggleActionError('save', errMsg);
+            }
 
             // Remember that an error occurred
             // so we can disable autosave
             // (avoids repeatedly refreshing the error message)
             view.errorOnLastSave = true;
         });
     }
```

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_response_editor.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_rubric.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_self.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_self.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_staff.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_staff.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_staff_area.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/lms/oa_training.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/lms/oa_training.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/oa_server.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/oa_server.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -242,15 +242,15 @@
             }).done(function(data) {
                 if (data.success) {
                     defer.resolve();
                 } else {
                     defer.rejectWith(this, [data.msg]);
                 }
             }).fail(function() {
-                defer.rejectWith(this, [gettext('This response could not be saved.')]);
+                defer.rejectWith(this, [gettext('Please check your internet connection.')]);
             });
         }).promise();
     }
 
     /**
      * Submit feedback on assessments to the XBlock.
      *
```

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/oa_shared.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/oa_shared.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_container.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_container.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_container_item.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_container_item.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_fields.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_settings.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js` & `ora2-5.1.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/student_training_mixin.py` & `ora2-5.1.0/openassessment/xblock/student_training_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/studio_mixin.py` & `ora2-5.1.0/openassessment/xblock/studio_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/submission_mixin.py` & `ora2-5.1.0/openassessment/xblock/submission_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,19 +254,19 @@
                 # Emit analytics event...
                 self.runtime.publish(
                     self,
                     "openassessmentblock.save_submission",
                     {"saved_response": self.saved_response}
                 )
             except Exception:  # pylint: disable=broad-except
-                return {'success': False, 'msg': self._("This response could not be saved.")}
+                return {'success': False, 'msg': self._("Please contact support staff.")}
             else:
                 return {'success': True, 'msg': ''}
         else:
-            return {'success': False, 'msg': self._("This response was not submitted.")}
+            return {'success': False, 'msg': self._("Submission data missing. Please contact support staff.")}
 
     @XBlock.json_handler
     def save_files_descriptions(self, data, suffix=''):  # pylint: disable=unused-argument
         """
         Save the metadata for each uploaded file.
 
         Args:
@@ -783,16 +783,16 @@
     def save_status(self):
         """
         Return a string indicating whether the response has been saved.
 
         Returns:
             unicode
         """
-        return self._('This response has been saved but not submitted.') if self.has_saved else self._(
-            'This response has not been saved.')
+        return self._('Draft saved!') if self.has_saved else self._(
+            'Response not started.')
 
     @XBlock.handler
     def render_submission(self, data, suffix=''):  # pylint: disable=unused-argument
         """Renders the Submission HTML section of the XBlock
 
         Generates the submission HTML for the first section of an Open
         Assessment XBlock. See OpenAssessmentBlock.render_assessment() for
```

### Comparing `ora2-5.0.4/openassessment/xblock/team_mixin.py` & `ora2-5.1.0/openassessment/xblock/team_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/team_workflow_mixin.py` & `ora2-5.1.0/openassessment/xblock/team_workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/user_data.py` & `ora2-5.1.0/openassessment/xblock/user_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/validation.py` & `ora2-5.1.0/openassessment/xblock/validation.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/workflow_mixin.py` & `ora2-5.1.0/openassessment/xblock/workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/openassessment/xblock/xml.py` & `ora2-5.1.0/openassessment/xblock/xml.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/ora2.egg-info/PKG-INFO` & `ora2-5.1.0/ora2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.4
+Version: 5.1.0
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.4/ora2.egg-info/SOURCES.txt` & `ora2-5.1.0/ora2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -350,26 +350,33 @@
 openassessment/xblock/static/css/lib/backgrid/backgrid.css
 openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
 openassessment/xblock/static/dist/manifest.json
 openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
 openassessment/xblock/static/dist/openassessment-editor-textarea.js
 openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
 openassessment/xblock/static/dist/openassessment-editor-tinymce.js
+openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.css
+openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js
 openassessment/xblock/static/dist/openassessment-lms.css
 openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
 openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
 openassessment/xblock/static/dist/openassessment-lms.js
 openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
 openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
+openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css
+openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js
 openassessment/xblock/static/dist/openassessment-ltr.css
 openassessment/xblock/static/dist/openassessment-ltr.js
 openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
 openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
 openassessment/xblock/static/dist/openassessment-rtl.css
+openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css
+openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js
 openassessment/xblock/static/dist/openassessment-rtl.js
+openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js
 openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
 openassessment/xblock/static/dist/openassessment-studio.js
 openassessment/xblock/static/js/lib/backgrid/backgrid.js
 openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
 openassessment/xblock/static/js/src/lms_index.js
 openassessment/xblock/static/js/src/oa_server.js
 openassessment/xblock/static/js/src/oa_shared.js
```

### Comparing `ora2-5.0.4/requirements/test.in` & `ora2-5.1.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.4/setup.py` & `ora2-5.1.0/setup.py`

 * *Files identical despite different names*

