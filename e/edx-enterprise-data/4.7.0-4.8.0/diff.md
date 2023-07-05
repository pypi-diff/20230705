# Comparing `tmp/edx-enterprise-data-4.7.0.tar.gz` & `tmp/edx-enterprise-data-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-4.7.0.tar", last modified: Tue Jun 20 14:27:08 2023, max compression
+gzip compressed data, was "edx-enterprise-data-4.8.0.tar", last modified: Wed Jul  5 14:41:50 2023, max compression
```

## Comparing `edx-enterprise-data-4.7.0.tar` & `edx-enterprise-data-4.8.0.tar`

### file list

```diff
@@ -1,175 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.321462 edx-enterprise-data-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)    17098 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-20 14:27:08.321462 edx-enterprise-data-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6803 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-20 14:27:08.000000 edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    18637 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.301461 edx-enterprise-data-4.7.0/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.305462 edx-enterprise-data-4.7.0/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.305462 edx-enterprise-data-4.7.0/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.305462 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.309461 edx-enterprise-data-4.7.0/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-20 14:26:57.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0030_auto_20230609_1353.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/0031_auto_20230615_0705.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12160 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.309461 edx-enterprise-data-4.7.0/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    12007 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.313462 edx-enterprise-data-4.7.0/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.317462 edx-enterprise-data-4.7.0/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.317462 edx-enterprise-data-4.7.0/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.317462 edx-enterprise-data-4.7.0/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.317462 edx-enterprise-data-4.7.0/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:27:08.321462 edx-enterprise-data-4.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 14:27:08.321462 edx-enterprise-data-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-20 14:26:58.000000 edx-enterprise-data-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.948232 edx-enterprise-data-4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    17219 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-05 14:41:50.948232 edx-enterprise-data-4.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.916232 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6857 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-05 14:41:50.000000 edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18637 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.920232 edx-enterprise-data-4.8.0/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.924232 edx-enterprise-data-4.8.0/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.924232 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0030_auto_20230609_1353.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0031_auto_20230615_0705.py
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/0032_auto_20230704_0818.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12280 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.932232 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12241 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.936232 edx-enterprise-data-4.8.0/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.936232 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.936232 edx-enterprise-data-4.8.0/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.940232 edx-enterprise-data-4.8.0/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.940232 edx-enterprise-data-4.8.0/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.940232 edx-enterprise-data-4.8.0/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.944232 edx-enterprise-data-4.8.0/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9493 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13860 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 14:41:50.944232 edx-enterprise-data-4.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 14:41:50.948232 edx-enterprise-data-4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-07-05 14:41:45.000000 edx-enterprise-data-4.8.0/setup.py
```

### Comparing `edx-enterprise-data-4.7.0/CHANGELOG.rst` & `edx-enterprise-data-4.8.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
+[4.8.0] - 2023-07-4
+---------------------
+  * Added new fields for offer utilization in OCM and Exec-Ed product types.
+
+
 [4.7.0] - 2023-06-20
 ---------------------
   * Added new fields for subsidy and product_line in EnterpriseLearnerEnrollmentViewSet.
 
 
 [4.6.10] - 2023-06-20
 ---------------------
```

### Comparing `edx-enterprise-data-4.7.0/LICENSE` & `edx-enterprise-data-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/MANIFEST.in` & `edx-enterprise-data-4.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/PKG-INFO` & `edx-enterprise-data-4.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.7.0
+Version: 4.8.0
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.7.0/README.md` & `edx-enterprise-data-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/PKG-INFO` & `edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.7.0
+Version: 4.8.0
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.7.0/edx_enterprise_data.egg-info/SOURCES.txt` & `edx-enterprise-data-4.8.0/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 enterprise_data/migrations/0025_auto_20210703_1854.py
 enterprise_data/migrations/0026_auto_20210916_0414.py
 enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
 enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
 enterprise_data/migrations/0029_enterpriseoffer.py
 enterprise_data/migrations/0030_auto_20230609_1353.py
 enterprise_data/migrations/0031_auto_20230615_0705.py
+enterprise_data/migrations/0032_auto_20230704_0818.py
 enterprise_data/migrations/__init__.py
 enterprise_data/settings/__init__.py
 enterprise_data/settings/test.py
 enterprise_data/tests/__init__.py
 enterprise_data/tests/mixins.py
 enterprise_data/tests/test_clients.py
 enterprise_data/tests/test_filters.py
```

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v0/serializers.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v0/urls.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v0/views.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v1/serializers.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v1/urls.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/api/v1/views.py` & `edx-enterprise-data-4.8.0/enterprise_data/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/clients.py` & `edx-enterprise-data-4.8.0/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/filters.py` & `edx-enterprise-data-4.8.0/enterprise_data/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/fixtures/enterprise_enrollment.json` & `edx-enterprise-data-4.8.0/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/fixtures/enterprise_user.json` & `edx-enterprise-data-4.8.0/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_dummy_data.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_offer.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/create_enterprise_user.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx-enterprise-data-4.8.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0001_initial.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0011_enterpriseuser.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0030_auto_20230609_1353.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0030_auto_20230609_1353.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/migrations/0031_auto_20230615_0705.py` & `edx-enterprise-data-4.8.0/enterprise_data/migrations/0031_auto_20230615_0705.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/models.py` & `edx-enterprise-data-4.8.0/enterprise_data/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,16 @@
     discount_type = models.CharField(max_length=64, null=True)
     discount_value = models.FloatField(null=True)
     max_discount = models.FloatField(null=True)
     total_discount_ecommerce = models.FloatField(null=True)
     amount_of_offer_spent = models.FloatField(null=True)
     percent_of_offer_spent = models.FloatField(null=True)
     remaining_balance = models.FloatField(null=True)
+    amount_offer_spent_ocm = models.FloatField(null=True)
+    amount_offer_spent_exec_ed = models.FloatField(null=True)
 
     def __str__(self):
         """
         Return a human-readable string representation of the object.
         """
         return f'<Enterprise Offer {self.offer_id} for {self.enterprise_name}>'
```

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/settings/test.py` & `edx-enterprise-data-4.8.0/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/signals.py` & `edx-enterprise-data-4.8.0/enterprise_data/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/api/v0/test_serializers.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/test_serializers.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/api/v1/test_views.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/api/v1/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/mixins.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/test_clients.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/test_filters.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/test_models.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/test_utils.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,20 @@
     )
     percent_of_offer_spent = factory.lazy_attribute(
         lambda x: round(x.amount_of_offer_spent / x.max_discount, 2)
     )
     remaining_balance = factory.lazy_attribute(
         lambda x: round(x.max_discount - x.amount_of_offer_spent, 2)
     )
+    amount_offer_spent_ocm = factory.lazy_attribute(
+        lambda x: round(x.amount_of_offer_spent / 2, 2)
+    )
+    amount_offer_spent_exec_ed = factory.lazy_attribute(
+        lambda x: round(x.amount_of_offer_spent / 2, 2)
+    )
 
 
 def get_dummy_enterprise_api_data(**kwargs):
     """
     DRY method to get enterprise dummy data.
 
     Get dummy data for an enterprise from `enterprise-customer` API.
```

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/tests/test_views.py` & `edx-enterprise-data-4.8.0/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data/utils.py` & `edx-enterprise-data-4.8.0/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/admin.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0001_initial.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/models.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/rules.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/tests/factories.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_data_roles/tests/test_models.py` & `edx-enterprise-data-4.8.0/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/clients/__init__.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/clients/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,22 @@
 
 import os
 from datetime import datetime, timedelta
 from functools import wraps
 from urllib.parse import parse_qs, urljoin, urlparse
 from edx_rest_api_client.client import get_oauth_access_token
 
+import logging
 import requests
 
+from enterprise_reporting.utils import retry_on_exception
+
+
+LOGGER = logging.getLogger(__name__)
+
 
 class EdxOAuth2APIMixin:
     """
     Base API Client Mixin for accessing edX IDA API endpoints.
     """
     @staticmethod
     def refresh_token(func):
@@ -49,14 +55,15 @@
         Connect to the REST API.
         """
         self.client_id = client_id or os.environ.get('LMS_OAUTH_KEY')
         self.client_secret = client_secret or os.environ.get('LMS_OAUTH_SECRET')
         self.expires_at = datetime.utcnow()
         self.access_token = None
 
+    @retry_on_exception(max_retries=3, delay=2, backoff=2)
     def connect(self):
         """
         Connect to the REST API, authenticating with an access token retrieved with our client credentials.
         """
         url = urljoin(f'{self.LMS_OAUTH_HOST}/', 'oauth2/access_token')
         self.access_token, self.expires_at = get_oauth_access_token(url, self.client_id, self.client_secret)
```

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/clients/enterprise.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/clients/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/clients/s3.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/clients/snowflake.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/clients/vertica.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/delivery_method.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/external_resource_link_report.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx-enterprise-data-4.8.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/reporter.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/send_enterprise_reports.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_clients.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_delivery_method.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_enterprise_client.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_external_link_report.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_reporter.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/test_utils.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -291,7 +291,28 @@
         attachments = utils.prepare_attachments(attachment_data)
 
         for index, filename in enumerate([file_on_filesystem_name, 'my_test.csv']):
             expected_header = 'attachment; filename="{}"'.format(
                 os.path.basename(filename)
             )
             assert attachments[index].get('Content-Disposition') == expected_header
+
+
+class TestRetryOnException(unittest.TestCase):
+    """
+    Test that the decorator `retry_on_exception` works correctly.
+    """
+
+    def test_retry_on_exception(self):
+        """
+        retry_on_exception should retry the function the given
+        number of times if an exception is raised.
+        """
+
+        @utils.retry_on_exception(max_retries=1, delay=1, backoff=1)
+        def raise_exception():
+            raise Exception('test')
+
+        # The function should be retried once after an exception,
+        # then raise the exception.
+        with self.assertRaises(Exception):
+            raise_exception()
```

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/tests/utils.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/enterprise_reporting/utils.py` & `edx-enterprise-data-4.8.0/enterprise_reporting/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -347,7 +347,59 @@
     """
     enterprise_customer_catalogs = {'results': [
         {'uuid': catalog['uuid']}
         for catalog in reporting_config.get('enterprise_customer_catalogs', [])
         ]
     }
     return enterprise_customer_catalogs
+
+
+def retry_on_exception(max_retries=3, delay=2, backoff=2):
+    """
+    Decorator to retry a function on exception with exponential backoff. The
+    function will be retried on exception up to max_retries times. The delay
+    between retries will increase exponentially with each retry.
+
+    :param max_retries: maximum number of retries
+    :param delay: initial delay in seconds
+    :param backoff: backoff multiplier e.g. value of 2 will double the delay
+
+    :return: decorator
+    """
+
+    def backoff_time(retry_count):
+        """
+        Calculate wait time using exponential backoff formula
+
+        :param retry_count: number of retries
+        :return: wait time
+        """
+        return delay * (backoff ** (retry_count - 1))
+
+    def wait(wait_time):
+        """
+        Wait for wait_time seconds using time.sleep
+
+        :param wait_time: time to wait in seconds
+        :return: None
+        """
+        import time
+        time.sleep(wait_time)
+
+    def decorator_retry(func):
+        def wrapper(*args, **kwargs):
+            retry_count = 0
+            while retry_count < max_retries:  # retry loop
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    LOGGER.info(
+                        'Exception raised while calling %s. Retrying: %s',
+                        func.__name__,
+                        str(e),
+                    )
+                    retry_count += 1
+                    time = backoff_time(retry_count)
+                    wait(time)
+            return func(*args, **kwargs)  # last attempt (don't wait)
+        return wrapper
+    return decorator_retry
```

### Comparing `edx-enterprise-data-4.7.0/requirements/base.txt` & `edx-enterprise-data-4.8.0/requirements/base.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
```

### Comparing `edx-enterprise-data-4.7.0/requirements/ci.txt` & `edx-enterprise-data-4.8.0/requirements/ci.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # via virtualenv
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via tox
-platformdirs==3.5.3
+platformdirs==3.6.0
     # via virtualenv
 pluggy==1.0.0
     # via tox
 py==1.11.0
     # via tox
 six==1.16.0
     # via tox
@@ -27,9 +27,9 @@
 tox==3.28.0
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/ci.in
     #   tox-battery
 tox-battery==0.6.1
     # via -r requirements/ci.in
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via tox
```

### Comparing `edx-enterprise-data-4.7.0/requirements/constraints.txt` & `edx-enterprise-data-4.8.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/requirements/dev.txt` & `edx-enterprise-data-4.8.0/requirements/dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
 bleach==6.0.0
     # via readme-renderer
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 build==0.10.0
     # via pip-tools
 celery==4.4.7
@@ -152,15 +152,15 @@
     #   snowflake-connector-python
     #   tox
     #   virtualenv
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
 importlib-resources==5.12.0
     # via keyring
 interchange==2021.0.4
     # via py2neo
@@ -220,15 +220,15 @@
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
 pip-tools==6.13.0
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.5.3
+platformdirs==3.6.0
     # via
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via
     #   diff-cover
     #   tox
@@ -306,15 +306,15 @@
     #   interchange
     #   snowflake-connector-python
 pyyaml==5.4.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
 requests==2.31.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   requests-toolbelt
@@ -405,15 +405,15 @@
     #   twine
 vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via tox
 webencodings==0.5.1
     # via bleach
 wheel==0.40.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
```

### Comparing `edx-enterprise-data-4.7.0/requirements/quality.txt` & `edx-enterprise-data-4.8.0/requirements/quality.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 astroid==2.15.5
     # via
     #   pylint
     #   pylint-celery
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
 bleach==6.0.0
     # via readme-renderer
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 build==0.10.0
     # via pip-tools
 celery==4.4.7
@@ -165,15 +165,15 @@
     # via -r requirements/test.in
 freezegun==1.2.2
     # via -r requirements/test.in
 idna==3.4
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==6.6.0
+importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
 importlib-resources==5.12.0
     # via keyring
 iniconfig==2.0.0
     # via pytest
@@ -238,15 +238,15 @@
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
 pip-tools==6.13.0
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.9.6
     # via twine
-platformdirs==3.5.3
+platformdirs==3.6.0
     # via
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via
     #   diff-cover
     #   pytest
@@ -335,15 +335,15 @@
     #   snowflake-connector-python
 pyyaml==5.4.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
     #   responses
-readme-renderer==37.3
+readme-renderer==40.0
     # via twine
 requests==2.31.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   requests-toolbelt
@@ -444,15 +444,15 @@
     #   twine
 vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via tox
 webencodings==0.5.1
     # via bleach
 wheel==0.40.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
```

### Comparing `edx-enterprise-data-4.7.0/requirements/reporting.in` & `edx-enterprise-data-4.8.0/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.7.0/requirements/test-master.txt` & `edx-enterprise-data-4.8.0/requirements/test-master.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
```

### Comparing `edx-enterprise-data-4.7.0/requirements/test-reporting.txt` & `edx-enterprise-data-4.8.0/requirements/test-reporting.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     # via
     #   oscrypto
     #   snowflake-connector-python
 atomicwrites==1.4.1
     # via pytest
 attrs==23.1.0
     # via pytest
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
@@ -94,15 +94,15 @@
     # via py2neo
 paramiko==3.2.0
     # via -r requirements/reporting.in
 pbr==5.11.1
     # via mock
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.5.3
+platformdirs==3.6.0
     # via virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 py==1.11.0
     # via
@@ -197,12 +197,12 @@
     #   snowflake-connector-python
 vertica-python==1.3.2
     # via -r requirements/reporting.in
 vine==1.3.0
     # via
     #   amqp
     #   celery
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via tox
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `edx-enterprise-data-4.7.0/requirements/test.txt` & `edx-enterprise-data-4.8.0/requirements/test.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     # via kombu
 asgiref==3.7.2
     # via django
 asn1crypto==1.5.1
     # via
     #   oscrypto
     #   snowflake-connector-python
-awscli==1.27.153
+awscli==1.27.156
     # via -r requirements/reporting.in
 bcrypt==4.0.1
     # via paramiko
 billiard==3.6.4.0
     # via celery
-boto3==1.26.153
+boto3==1.26.156
     # via -r requirements/reporting.in
-botocore==1.29.153
+botocore==1.29.156
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==4.4.7
     # via -r requirements/reporting.in
 certifi==2023.5.7
```

### Comparing `edx-enterprise-data-4.7.0/setup.py` & `edx-enterprise-data-4.8.0/setup.py`

 * *Files identical despite different names*

