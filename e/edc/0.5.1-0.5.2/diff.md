# Comparing `tmp/edc-0.5.1.tar.gz` & `tmp/edc-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.1.tar", last modified: Sun Jul  2 20:54:32 2023, max compression
+gzip compressed data, was "edc-0.5.2.tar", last modified: Wed Jul  5 01:03:18 2023, max compression
```

## Comparing `edc-0.5.1.tar` & `edc-0.5.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.127756 edc-0.5.1/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.1/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.1/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.1/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    40752 2023-07-02 19:04:41.000000 edc-0.5.1/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.1/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.1/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-02 20:54:32.127884 edc-0.5.1/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.1/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.114213 edc-0.5.1/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.117625 edc-0.5.1/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.1/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.1/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.1/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.118262 edc-0.5.1/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.1/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.1/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.1/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.1/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.119337 edc-0.5.1/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.1/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.123174 edc-0.5.1/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.1/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.1/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.1/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.1/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.1/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.1/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.1/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.1/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.1/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.1/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.1/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.1/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.1/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.1/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.1/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.1/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.1/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.1/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.1/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.124046 edc-0.5.1/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-02 20:54:32.000000 edc-0.5.1/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-02 20:54:32.000000 edc-0.5.1/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-02 20:54:32.000000 edc-0.5.1/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.1/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1915 2023-07-02 20:54:32.000000 edc-0.5.1/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-02 20:54:32.000000 edc-0.5.1/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.124156 edc-0.5.1/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.1/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.1/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.127206 edc-0.5.1/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.1/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.1/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.1/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.1/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.1/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.1/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.1/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.1/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.1/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.1/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.1/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2986 2023-07-02 20:54:32.128349 edc-0.5.1/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-02 20:54:32.127522 edc-0.5.1/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.1/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.1/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.162206 edc-0.5.2/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.2/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.2/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.2/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    41042 2023-07-05 01:03:10.000000 edc-0.5.2/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.2/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.2/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-05 01:03:18.162322 edc-0.5.2/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37628 2023-06-23 15:02:46.000000 edc-0.5.2/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.149248 edc-0.5.2/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.152131 edc-0.5.2/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.2/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.152788 edc-0.5.2/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.2/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.2/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.2/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.2/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.153867 edc-0.5.2/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.2/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.157894 edc-0.5.2/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.2/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.2/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.2/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.2/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.2/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.2/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.2/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.2/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.2/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.2/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.2/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.2/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.2/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.2/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.2/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.2/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.2/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.2/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.2/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.158749 edc-0.5.2/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38490 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.2/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-05 01:03:18.000000 edc-0.5.2/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.158865 edc-0.5.2/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.2/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.2/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.161656 edc-0.5.2/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.2/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.2/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.2/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.2/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.2/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.2/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.2/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.2/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.2/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.2/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.2/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2987 2023-07-05 01:03:18.162722 edc-0.5.2/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-05 01:03:18.161974 edc-0.5.2/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.2/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.2/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.1/.gitignore` & `edc-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/.pre-commit-config.yaml` & `edc-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/CHANGES` & `edc-0.5.2/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changes
 -------
 
-0.5.0
+0.5.2
+-----
+- force all models to use `objects` as default manager (edc-model)
+- add new mixins to handle redirects, delete button (edc-model-admin)
+- update admin mixin to handle fks/m2ms in modelform (edc-site)
+- move managers from fields mixin to screening_model_mixin (edc-screening)
+
+
+0.5.1
 ------
 - add additonal validation to check screening identifier and the screening
   eligibility boolean. (edc-cosent)
 - add mixin to redirect all forms to a selected changelist (edc-model-admin)
 - improve redirect on delete (edc-model-admin)
```

### Comparing `edc-0.5.1/LICENSE` & `edc-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/PKG-INFO` & `edc-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.1
+Version: 0.5.2
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.1/README.rst` & `edc-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/nginx/edc-uat.conf` & `edc-0.5.2/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/nginx/edc.conf` & `edc-0.5.2/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/scripts/dev_repos.sh` & `edc-0.5.2/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/scripts/update_edc.sh` & `edc-0.5.2/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/systemd/celery-uat.service` & `edc-0.5.2/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/bin/systemd/celery.service` & `edc-0.5.2/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/Makefile` & `edc-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/README.rst` & `edc-0.5.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/backup.rst` & `edc-0.5.2/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/celery.rst` & `edc-0.5.2/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/conda.rst` & `edc-0.5.2/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/conf.py` & `edc-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/configure_web_services.rst` & `edc-0.5.2/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/deploy_new_droplet.rst` & `edc-0.5.2/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/exporting_encrypted_data.rst` & `edc-0.5.2/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/forms_reference.md` & `edc-0.5.2/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/landing_page.rst` & `edc-0.5.2/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/make.bat` & `edc-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/prepare_database.rst` & `edc-0.5.2/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/printing.rst` & `edc-0.5.2/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/docs/update_deployment.rst` & `edc-0.5.2/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/edc.egg-info/PKG-INFO` & `edc-0.5.2/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.1
+Version: 0.5.2
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.1/edc.egg-info/SOURCES.txt` & `edc-0.5.2/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/edc.egg-info/requires.txt` & `edc-0.5.2/edc.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,47 +22,47 @@
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
 edc-action-item==0.3.52
 edc-adherence==0.1.21
 edc-adverse-event==0.3.54
 edc-appointment==0.3.73
-edc-auth==0.3.60
+edc-auth==0.3.61
 edc-consent==0.3.46
 edc-constants==0.3.49
 edc-crf==0.3.43
 edc-dashboard==0.3.45
-edc-data-manager==0.3.53
+edc-data-manager==0.3.54
 edc-device==0.3.11
 edc-document-status==0.1.4
 edc-dx==0.1.19
 edc-dx-review==0.1.39
 edc-egfr==0.1.11
 edc-export==0.3.26
 edc-facility==0.3.15
 edc-fieldsets==0.3.13
 edc-form-describer==0.3.14
 edc-form-label==0.3.9
 edc-form-validators==0.3.34
 edc-glucose==0.1.30
-edc-he==0.1.7
+edc-he==0.1.8
 edc-identifier==0.3.23
 edc-lab==0.3.43
 edc-lab-dashboard==0.3.11
 edc-lab-panel==0.1.15
 edc-lab-results==0.1.38
 edc-label==0.3.12
 edc-list-data==0.3.18
-edc-listboard==0.1.9
+edc-listboard==0.1.10
 edc-locator==0.3.23
 edc-ltfu==0.3.23
-edc-metadata==0.3.51
+edc-metadata==0.3.52
 edc-mnsi==0.1.16
-edc-model==0.3.30
-edc-model-admin==0.3.45
+edc-model==0.3.31
+edc-model-admin==0.3.46
 edc-model-fields==0.3.7
 edc-model-form==0.1.12
 edc-model-wrapper==0.3.10
 edc-navbar==0.3.16
 edc-notification==0.3.17
 edc-offstudy==0.3.32
 edc-pdf-reports==0.3.13
@@ -72,21 +72,21 @@
 edc-prn==0.3.13
 edc-protocol==0.3.9
 edc-protocol-incident==0.1.25
 edc-qol==0.1.14
 edc-randomization==0.3.46
 edc-reference==0.3.15
 edc-refusal==0.1.12
-edc-registration==0.3.28
+edc-registration==0.3.29
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
 edc-rx==0.1.6
-edc-screening==0.3.34
+edc-screening==0.3.35
 edc-search==0.3.7
-edc-sites==0.3.20
+edc-sites==0.3.21
 edc-subject-dashboard==0.3.36
 edc-subject-model-wrappers==0.3.15
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
 edc-unblinding==0.1.14
 edc-utils==0.3.20
 edc-visit-schedule==0.3.61
```

### Comparing `edc-0.5.1/image/icon-pycharm.png` & `edc-0.5.2/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/requirements.tests/edc.txt` & `edc-0.5.2/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/requirements.tests/edc_dev.txt` & `edc-0.5.2/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.1/setup.cfg` & `edc-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -51,47 +51,47 @@
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
 	edc-action-item==0.3.52
 	edc-adherence==0.1.21
 	edc-adverse-event==0.3.54
 	edc-appointment==0.3.73
-	edc-auth==0.3.60
+	edc-auth==0.3.61
 	edc-consent==0.3.46
 	edc-constants==0.3.49
 	edc-crf==0.3.43
 	edc-dashboard==0.3.45
-	edc-data-manager==0.3.53
+	edc-data-manager==0.3.54
 	edc-device==0.3.11
 	edc-document-status==0.1.4
 	edc-dx==0.1.19
 	edc-dx-review==0.1.39
 	edc-egfr==0.1.11
 	edc-export==0.3.26
 	edc-facility==0.3.15
 	edc-fieldsets==0.3.13
 	edc-form-describer==0.3.14
 	edc-form-label==0.3.9
 	edc-form-validators==0.3.34
 	edc-glucose==0.1.30
-	edc-he==0.1.7
+	edc-he==0.1.8
 	edc-identifier==0.3.23
 	edc-lab==0.3.43
 	edc-lab-dashboard==0.3.11
 	edc-lab-panel==0.1.15
 	edc-lab-results==0.1.38
 	edc-label==0.3.12
 	edc-list-data==0.3.18
-	edc-listboard==0.1.9
+	edc-listboard==0.1.10
 	edc-locator==0.3.23
 	edc-ltfu==0.3.23
-	edc-metadata==0.3.51
+	edc-metadata==0.3.52
 	edc-mnsi==0.1.16
-	edc-model==0.3.30
-	edc-model-admin==0.3.45
+	edc-model==0.3.31
+	edc-model-admin==0.3.46
 	edc-model-fields==0.3.7
 	edc-model-form==0.1.12
 	edc-model-wrapper==0.3.10
 	edc-navbar==0.3.16
 	edc-notification==0.3.17
 	edc-offstudy==0.3.32
 	edc-pdf-reports==0.3.13
@@ -101,21 +101,21 @@
 	edc-prn==0.3.13
 	edc-protocol==0.3.9
 	edc-protocol-incident==0.1.25
 	edc-qol==0.1.14
 	edc-randomization==0.3.46
 	edc-reference==0.3.15
 	edc-refusal==0.1.12
-	edc-registration==0.3.28
+	edc-registration==0.3.29
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
 	edc-rx==0.1.6
-	edc-screening==0.3.34
+	edc-screening==0.3.35
 	edc-search==0.3.7
-	edc-sites==0.3.20
+	edc-sites==0.3.21
 	edc-subject-dashboard==0.3.36
 	edc-subject-model-wrappers==0.3.15
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
 	edc-unblinding==0.1.14
 	edc-utils==0.3.20
 	edc-visit-schedule==0.3.61
```

### Comparing `edc-0.5.1/utils/get_edc_requirements.py` & `edc-0.5.2/utils/get_edc_requirements.py`

 * *Files identical despite different names*

