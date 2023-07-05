# Comparing `tmp/django-mass-migration-0.1.6.tar.gz` & `tmp/django-mass-migration-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.1.6.tar", last modified: Mon Jul  3 16:31:49 2023, max compression
+gzip compressed data, was "django-mass-migration-0.1.7.tar", last modified: Wed Jul  5 11:12:17 2023, max compression
```

## Comparing `django-mass-migration-0.1.6.tar` & `django-mass-migration-0.1.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.737513 django-mass-migration-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-03 16:31:49.737513 django-mass-migration-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.729513 django-mass-migration-0.1.6/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-03 16:31:49.000000 django-mass-migration-0.1.6/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-03 16:31:49.000000 django-mass-migration-0.1.6/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:31:49.000000 django-mass-migration-0.1.6/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 16:31:49.000000 django-mass-migration-0.1.6/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 16:31:49.000000 django-mass-migration-0.1.6/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.729513 django-mass-migration-0.1.6/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.729513 django-mass-migration-0.1.6/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.729513 django-mass-migration-0.1.6/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/massmigration/migration_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/massmigration/run_migration.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/templates/migration_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/migration_templates/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/migration_templates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/templates/migration_templates/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.733513 django-mass-migration-0.1.6/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/massmigration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:31:49.737513 django-mass-migration-0.1.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-03 16:31:46.000000 django-mass-migration-0.1.6/scripts/release.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:31:49.737513 django-mass-migration-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-03 16:31:48.000000 django-mass-migration-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 11:12:17.000000 django-mass-migration-0.1.7/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.083212 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-05 11:12:10.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/migration_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/templates/migration_templates/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/massmigration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-07-05 11:12:11.000000 django-mass-migration-0.1.7/scripts/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 11:12:17.087212 django-mass-migration-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-05 11:12:15.000000 django-mass-migration-0.1.7/setup.py
```

### Comparing `django-mass-migration-0.1.6/LICENSE` & `django-mass-migration-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/PKG-INFO` & `django-mass-migration-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.6/README.md` & `django-mass-migration-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.1.7/django_mass_migration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-mass-migration-0.1.6/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.1.7/django_mass_migration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/admin.py` & `django-mass-migration-0.1.7/massmigration/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Third party
 from django.contrib import admin
+from django.contrib.admin.templatetags.admin_list import _boolean_icon
 
 # Mass Migration
 from .loader import store
 from .models import MigrationRecord
 
 
 class MigrationRecordAdmin(admin.ModelAdmin):
     """ Custom admin class for the Migration model. """
 
     ordering = ("-initiated_at",)
-    list_display = ("key", "initiated_at", "is_applied", "applied_at", "was_faked")
+    list_display = ("key", "initiated_at", "is_applied", "successful", "applied_at", "was_faked")
     list_filter = ("app_label", "is_applied", "was_faked")
     readonly_fields = ("app_label", "name", "description")
 
     def description(self, obj):
         migration = store.by_key[obj.key]
         return migration.description
 
+    def successful(self, obj):
+        return _boolean_icon((not obj.has_error) if obj.is_applied else None)
+
 
 admin.site.register(MigrationRecord, MigrationRecordAdmin)
```

### Comparing `django-mass-migration-0.1.6/massmigration/backends/base.py` & `django-mass-migration-0.1.7/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/backends/djangae.py` & `django-mass-migration-0.1.7/massmigration/backends/djangae.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/enforcement.py` & `django-mass-migration-0.1.7/massmigration/enforcement.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/exceptions.py` & `django-mass-migration-0.1.7/massmigration/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/loader.py` & `django-mass-migration-0.1.7/massmigration/loader.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.1.7/massmigration/management/commands/makemassmigration.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/migrations.py` & `django-mass-migration-0.1.7/massmigration/migrations.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/models.py` & `django-mass-migration-0.1.7/massmigration/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,12 +67,12 @@
         """ Given a 2-part migration identifier, return the single string object which we use as
             the `key` field value.
         """
         assert len(name_tuple) == 2
         return ":".join(name_tuple)
 
     def status(self):
-        if self.is_applied:
-            return self.Status.APPLIED
         if self.has_error:
             return self.Status.ERRORED
+        if self.is_applied:
+            return self.Status.APPLIED
         return self.Status.RUNNING
```

### Comparing `django-mass-migration-0.1.6/massmigration/record_cache.py` & `django-mass-migration-0.1.7/massmigration/record_cache.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.1.7/massmigration/templates/massmigration/base.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.1.7/massmigration/templates/massmigration/delete_migration.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.1.7/massmigration/templates/massmigration/manage_migrations.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/massmigration/migration_detail.html` & `django-mass-migration-0.1.7/massmigration/templates/massmigration/migration_detail.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/migration_templates/custom.py` & `django-mass-migration-0.1.7/massmigration/templates/migration_templates/custom.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/migration_templates/mapper.py` & `django-mass-migration-0.1.7/massmigration/templates/migration_templates/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/templates/migration_templates/simple.py` & `django-mass-migration-0.1.7/massmigration/templates/migration_templates/simple.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/utils/functional.py` & `django-mass-migration-0.1.7/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/utils/transaction.py` & `django-mass-migration-0.1.7/massmigration/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/massmigration/views.py` & `django-mass-migration-0.1.7/massmigration/views.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/scripts/release.py` & `django-mass-migration-0.1.7/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.1.6/setup.py` & `django-mass-migration-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # TODO: possibly make the dependency on djangae optional
 EXTRAS = {}
 
 
 setup(
     name=NAME,
-    version="v0.1.6",
+    version="v0.1.7",
     packages=PACKAGES,
     author=AUTHOR,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     keywords=["django", "djangae", "django-gcloud-connectors", "Google App Engine"],
     url=URL,
```

