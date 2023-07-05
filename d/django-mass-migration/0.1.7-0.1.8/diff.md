# Comparing `tmp/django-mass-migration-0.1.7.tar.gz` & `tmp/django-mass-migration-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.1.7.tar", last modified: Wed Jul  5 11:12:17 2023, max compression
+gzip compressed data, was "django-mass-migration-0.1.8.tar", last modified: Wed Jul  5 11:17:38 2023, max compression
```

## Comparing `django-mass-migration-0.1.7.tar` & `django-mass-migration-0.1.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/migration_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/run_migration.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/migration_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 11:12:15.000000 django-mass-migration-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.547256 django-mass-migration-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:17:38.547256 django-mass-migration-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:17:38.000000 django-mass-migration-0.1.8/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-05 11:17:38.000000 django-mass-migration-0.1.8/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:17:38.000000 django-mass-migration-0.1.8/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 11:17:38.000000 django-mass-migration-0.1.8/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 11:17:38.000000 django-mass-migration-0.1.8/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.539255 django-mass-migration-0.1.8/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.539255 django-mass-migration-0.1.8/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.539255 django-mass-migration-0.1.8/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/massmigration/migration_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/templates/migration_templates/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.543256 django-mass-migration-0.1.8/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/massmigration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:17:38.547256 django-mass-migration-0.1.8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-05 11:17:35.000000 django-mass-migration-0.1.8/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:17:38.547256 django-mass-migration-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 11:17:37.000000 django-mass-migration-0.1.8/setup.py
```

### Comparing `django-mass-migration-0.1.7/LICENSE` & `django-mass-migration-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/PKG-INFO` & `django-mass-migration-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.7/README.md` & `django-mass-migration-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.1.8/django_mass_migration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.7/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.1.8/django_mass_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/admin.py` & `django-mass-migration-0.1.8/massmigration/admin.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/backends/base.py` & `django-mass-migration-0.1.8/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/backends/djangae.py` & `django-mass-migration-0.1.8/massmigration/backends/djangae.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/enforcement.py` & `django-mass-migration-0.1.8/massmigration/enforcement.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/exceptions.py` & `django-mass-migration-0.1.8/massmigration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/loader.py` & `django-mass-migration-0.1.8/massmigration/loader.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.1.8/massmigration/management/commands/makemassmigration.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/migrations.py` & `django-mass-migration-0.1.8/massmigration/migrations.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/models.py` & `django-mass-migration-0.1.8/massmigration/models.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/record_cache.py` & `django-mass-migration-0.1.8/massmigration/record_cache.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.1.8/massmigration/templates/massmigration/base.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.1.8/massmigration/templates/massmigration/delete_migration.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.1.8/massmigration/templates/massmigration/manage_migrations.html`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 		</tr>
 	</thead>
 	<tbody>
 	{% for migration in migrations %}
 		<tr>
 			<td>{{migration.app_label}}</td>
 			<td><a href="{% url 'massmigration_detail' key=migration.key %}">{{migration.name}}</a></td>
-			<td>{% if migration.record.is_applied %}APPLIED{% elif migration.record.has_error %}ERRORED{% elif migration.record %}RUNNING{% else %}NOT RUN{% endif %}</td>
+			<td>{% if migration.record %}{{migration.record.status}}{% else %}NOT RUN{% endif %}</td>
 			<td>
 				{% if not migration.record %}<a href="{% url 'massmigration_run' key=migration.key %}">Run...</a>
 				{% else %}<a href="{% url 'massmigration_delete' key=migration.key %}">Delete...</a>
 				{% endif %}
 			</td>
 		</tr>
 	{% endfor %}
```

#### html2text {}

```diff
@@ -1,12 +1,9 @@
 {% extends "massmigration/base.html" %} {% block content %}
 ****** Migrations ******
-App                    Migration         Status                      Actions
-                                         {% if
-                                         migration.record.is_applied {% if not
-                                         %}APPLIED{% elif            migration.record
-{                      {                 migration.record.has_error  %}Run... {% else
-{migration.app_label}} {migration.name}} %}ERRORED{% elif            %}Delete... {%
-                                         migration.record %}RUNNING  endif %}
-                                         {% else %}NOT RUN{% endif
-                                         %}
+App                    Migration         Status                     Actions
+                                         {% if migration.record %}{ {% if not
+{                      {                 {migration.record.status}} migration.record
+{migration.app_label}} {migration.name}} {% else %}NOT RUN{% endif  %}Run... {% else
+                                         %}                         %}Delete... {%
+                                                                    endif %}
 {% endblock %}
```

### Comparing `django-mass-migration-0.1.7/massmigration/templates/massmigration/migration_detail.html` & `django-mass-migration-0.1.8/massmigration/templates/massmigration/migration_detail.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/migration_templates/custom.py` & `django-mass-migration-0.1.8/massmigration/templates/migration_templates/custom.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/migration_templates/mapper.py` & `django-mass-migration-0.1.8/massmigration/templates/migration_templates/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/templates/migration_templates/simple.py` & `django-mass-migration-0.1.8/massmigration/templates/migration_templates/simple.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/utils/functional.py` & `django-mass-migration-0.1.8/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/utils/transaction.py` & `django-mass-migration-0.1.8/massmigration/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/massmigration/views.py` & `django-mass-migration-0.1.8/massmigration/views.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/scripts/release.py` & `django-mass-migration-0.1.8/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.7/setup.py` & `django-mass-migration-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # TODO: possibly make the dependency on djangae optional
 EXTRAS = {}
 
 
 setup(
     name=NAME,
-    version="v0.1.7",
+    version="v0.1.8",
     packages=PACKAGES,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=["django", "djangae", "django-gcloud-connectors", "Google App Engine"],
     url=URL,
```

