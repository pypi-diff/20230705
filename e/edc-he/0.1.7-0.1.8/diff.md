# Comparing `tmp/edc-he-0.1.7.tar.gz` & `tmp/edc-he-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-he-0.1.7.tar", last modified: Wed May 24 17:41:29 2023, max compression
+gzip compressed data, was "edc-he-0.1.8.tar", last modified: Wed Jul  5 00:30:52 2023, max compression
```

## Comparing `edc-he-0.1.7.tar` & `edc-he-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.931835 edc-he-0.1.7/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.7/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.7/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.919433 edc-he-0.1.7/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.923578 edc-he-0.1.7/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:28.000000 edc-he-0.1.7/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.7/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:28.000000 edc-he-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.7/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.7/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.7/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.7/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.7/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-05-24 17:41:29.931927 edc-he-0.1.7/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.7/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.7/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.925661 edc-he-0.1.7/edc_he/
--rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      691 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      452 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8596 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      206 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/fieldsets.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.7/edc_he/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1474 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.926701 edc-he-0.1.7/edc_he/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    10762 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12993 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.927635 edc-he-0.1.7/edc_he/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      467 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5792 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/assets_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2176 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/education_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.927986 edc-he-0.1.7/edc_he/model_mixins/factory/
--rw-r--r--   0 erikvw     (501) staff       (20)      134 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/factory/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/factory/assets_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/factory/income_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3298 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/household_head_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      640 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/household_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2688 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/income_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2313 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/patient_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1812 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/model_mixins/property_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.928731 edc-he-0.1.7/edc_he/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      405 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4081 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/assets_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3562 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4418 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/income_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/patient_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1760 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/modeladmin_mixins/property_model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1022 2023-05-24 17:41:22.000000 edc-he-0.1.7/edc_he/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.929910 edc-he-0.1.7/edc_he/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.931353 edc-he-0.1.7/edc_he/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.7/edc_he/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.7/edc_he/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.931594 edc-he-0.1.7/edc_he/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4059 2023-05-24 16:43:28.000000 edc-he-0.1.7/edc_he/tests/tests/test_he.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.7/edc_he/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:41:29.926334 edc-he-0.1.7/edc_he.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-05-24 17:41:29.000000 edc-he-0.1.7/edc_he.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     2015 2023-05-24 17:41:29.000000 edc-he-0.1.7/edc_he.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:41:29.000000 edc-he-0.1.7/edc_he.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.7/edc_he.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-05-24 17:41:29.000000 edc-he-0.1.7/edc_he.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 16:43:28.000000 edc-he-0.1.7/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.7/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1134 2023-05-24 17:41:29.932283 edc-he-0.1.7/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659640 edc-he-0.1.8/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2021-08-23 17:45:53.000000 edc-he-0.1.8/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-08-23 17:45:53.000000 edc-he-0.1.8/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.648266 edc-he-0.1.8/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.651939 edc-he-0.1.8/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:43:28.000000 edc-he-0.1.8/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1842 2022-05-25 13:21:02.000000 edc-he-0.1.8/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:43:28.000000 edc-he-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:46:20.000000 edc-he-0.1.8/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.8/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 13:21:02.000000 edc-he-0.1.8/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-08-19 17:21:37.000000 edc-he-0.1.8/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 13:21:02.000000 edc-he-0.1.8/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-05 00:30:52.659716 edc-he-0.1.8/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      641 2021-08-23 17:45:53.000000 edc-he-0.1.8/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:46:20.000000 edc-he-0.1.8/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.654203 edc-he-0.1.8/edc_he/
+-rw-r--r--   0 erikvw     (501) staff       (20)       66 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      691 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      189 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8724 2023-07-05 00:30:45.000000 edc-he-0.1.8/edc_he/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      287 2023-07-05 00:30:45.000000 edc-he-0.1.8/edc_he/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      725 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/fieldsets.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2272 2022-05-25 13:21:02.000000 edc-he-0.1.8/edc_he/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1474 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.655184 edc-he-0.1.8/edc_he/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    10762 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12993 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.656318 edc-he-0.1.8/edc_he/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      467 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5792 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/assets_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2176 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/education_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.656701 edc-he-0.1.8/edc_he/model_mixins/factory/
+-rw-r--r--   0 erikvw     (501) staff       (20)      134 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1387 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/assets_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2624 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/factory/income_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3298 2023-05-24 22:27:22.000000 edc-he-0.1.8/edc_he/model_mixins/household_head_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      640 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/household_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2688 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/income_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2313 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/patient_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1812 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/model_mixins/property_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.657524 edc-he-0.1.8/edc_he/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      405 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4081 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/assets_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3562 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4418 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/income_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1621 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/patient_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1760 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/modeladmin_mixins/property_model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1022 2023-05-24 17:41:22.000000 edc-he-0.1.8/edc_he/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.657989 edc-he-0.1.8/edc_he/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659171 edc-he-0.1.8/edc_he/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      677 2022-10-05 19:09:01.000000 edc-he-0.1.8/edc_he/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      227 2022-09-25 18:36:50.000000 edc-he-0.1.8/edc_he/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.659427 edc-he-0.1.8/edc_he/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4059 2023-05-24 16:43:28.000000 edc-he-0.1.8/edc_he/tests/tests/test_he.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-08-23 17:45:53.000000 edc-he-0.1.8/edc_he/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 00:30:52.654787 edc-he-0.1.8/edc_he.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1484 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     2015 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-08-19 17:35:04.000000 edc-he-0.1.8/edc_he.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2023-07-05 00:30:52.000000 edc-he-0.1.8/edc_he.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1758 2023-05-24 16:43:28.000000 edc-he-0.1.8/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2329 2022-05-25 13:21:02.000000 edc-he-0.1.8/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1134 2023-07-05 00:30:52.660026 edc-he-0.1.8/setup.cfg
```

### Comparing `edc-he-0.1.7/.github/workflows/build.yml` & `edc-he-0.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/.gitignore` & `edc-he-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/.pre-commit-config.yaml` & `edc-he-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/LICENSE` & `edc-he-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/PKG-INFO` & `edc-he-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.7
+Version: 0.1.8
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-he-0.1.7/README.rst` & `edc-he-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/admin.py` & `edc-he-0.1.8/edc_he/admin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/choices.py` & `edc-he-0.1.8/edc_he/choices.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,20 @@
     SECONDARY,
     TERTIARY,
     WEEKLY,
     YEARLY,
 )
 
 from .constants import (
+    ALL_WINDOWS_SCREENED,
     BROTHER_SISTER,
     GRANDCHILD,
     PARENT,
     PARENTINLAW,
+    SOME_WINDOWS_SCREENED,
     SON_DAUGHTER,
     SON_DAUGHTERINLAW,
     WIFE_HUSBAND,
 )
 
 EDUCATION_CERTIFICATES_CHOICES = (
     (PRIMARY, "Primary Certificate"),
@@ -225,24 +227,25 @@
     ("4", "Iron/metal"),
     ("5", "Screens"),
     ("6", "No windows"),
     (OTHER, "Other, specify ..."),
 )
 
 WINDOW_SCREENING_CHOICES = (
-    ("1", "All windows screened"),
+    (ALL_WINDOWS_SCREENED, "All windows screened"),
     ("2", "No windows screened"),
-    ("3", "Some windows screened"),
+    (SOME_WINDOWS_SCREENED, "Some windows screened"),
 )
 
 WINDOW_SCREENING_TYPE_CHOICES = (
     ("1", "Wire mesh"),
     ("2", "Old bednet"),
     ("3", "No windows screened"),
     ("4", "No windows"),
+    (NOT_APPLICABLE, "Not applicable"),
 )
 
 FLOOR_MATERIALS_CHOICES = (
     ("6", "Earth, sand"),
     ("7", "Dung, wood, planks, palm, bamboo"),
     ("8", "Parquet, polished wood, vinyl, asphalt strips"),
     ("9", "Ceramic tiles"),
```

### Comparing `edc-he-0.1.7/edc_he/fieldsets.py` & `edc-he-0.1.8/edc_he/fieldsets.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/form_validators.py` & `edc-he-0.1.8/edc_he/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/list_data.py` & `edc-he-0.1.8/edc_he/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/migrations/0001_initial.py` & `edc-he-0.1.8/edc_he/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py` & `edc-he-0.1.8/edc_he/migrations/0002_historicalreligions_historicalnationalities_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/assets_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/assets_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/education_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/education_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/factory/assets_model_mixin_factory.py` & `edc-he-0.1.8/edc_he/model_mixins/factory/assets_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/factory/income_model_mixin_factory.py` & `edc-he-0.1.8/edc_he/model_mixins/factory/income_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/household_head_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/household_head_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/household_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/household_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/income_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/income_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/patient_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/patient_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/model_mixins/property_model_mixin.py` & `edc-he-0.1.8/edc_he/model_mixins/property_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/modeladmin_mixins/assets_model_admin_mixin.py` & `edc-he-0.1.8/edc_he/modeladmin_mixins/assets_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py` & `edc-he-0.1.8/edc_he/modeladmin_mixins/household_head_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/modeladmin_mixins/income_model_admin_mixin.py` & `edc-he-0.1.8/edc_he/modeladmin_mixins/income_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/modeladmin_mixins/patient_model_admin_mixin.py` & `edc-he-0.1.8/edc_he/modeladmin_mixins/patient_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/modeladmin_mixins/property_model_admin_mixin.py` & `edc-he-0.1.8/edc_he/modeladmin_mixins/property_model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/models.py` & `edc-he-0.1.8/edc_he/models.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/tests/etc/user-rsa-local-private.pem` & `edc-he-0.1.8/edc_he/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/tests/etc/user-rsa-restricted-private.pem` & `edc-he-0.1.8/edc_he/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/tests/forms.py` & `edc-he-0.1.8/edc_he/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he/tests/tests/test_he.py` & `edc-he-0.1.8/edc_he/tests/tests/test_he.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/edc_he.egg-info/PKG-INFO` & `edc-he-0.1.8/edc_he.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-he
-Version: 0.1.7
+Version: 0.1.8
 Summary: Base django classes for health economics
 Home-page: https://github.com/clinicedc/edc-he
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc health economics,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-he-0.1.7/edc_he.egg-info/SOURCES.txt` & `edc-he-0.1.8/edc_he.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/pyproject.toml` & `edc-he-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/runtests.py` & `edc-he-0.1.8/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-he-0.1.7/setup.cfg` & `edc-he-0.1.8/setup.cfg`

 * *Files identical despite different names*

