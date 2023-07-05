# Comparing `tmp/tutor-contrib-aspects-0.4.0.tar.gz` & `tmp/tutor-contrib-aspects-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.4.0.tar", last modified: Tue Jul  4 13:19:48 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.5.0.tar", last modified: Wed Jul  5 16:47:54 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.4.0.tar` & `tutor-contrib-aspects-0.5.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.723647 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-04 13:19:48.000000 tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.727648 tutor-contrib-aspects-0.4.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.731648 tutor-contrib-aspects-0.4.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.735648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.739648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.719647 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 13:19:48.743648 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-04 13:19:40.000000 tutor-contrib-aspects-0.4.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.4.0/PKG-INFO` & `tutor-contrib-aspects-0.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: tutor-contrib-aspects
-Version: 0.4.0
-Summary: Aspects plugin for Tutor
-Home-page: https://github.com/open-craft/tutor-contrib-aspects
-Author: The Open edX Community
-License: AGPLv3
-Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
-Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-
 The Aspects plugin for Tutor
 ============================
 
 Aspects Learner Analytics combines several free, open source, tools to add analytics and reporting capabilities to the Open edX platform. This plugin offers easy installation, configuration, and deployment of these tools using `Tutor <https://docs.tutor.overhang.io>`__. The tools Aspects uses are:
 
 - `ClickHouse <https://clickhouse.com>`__, a fast, scalable analytics database that can be run anywhere
 - `Apache Superset <https://superset.apache.org>`__, a data visualization platform and data API
@@ -207,11 +186,27 @@
         "sk": {"flag": "sk", "name": "Slovak"},
         "sl": {"flag": "si", "name": "Slovenian"},
         "nl": {"flag": "nl", "name": "Dutch"},
     }
 
 Where the first key is the abbreviation of the language to use, "flag" is which flag icon is displayed in the user interface for choosing the language, and "name" is the displayed name for that language. The mapping above shows all of the current languages supported by Superset, but please note that different languages have different levels of completion and support at this time.
 
+
+Extending the DBT project
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+To extend the DBT project there are multiple options:
+
+    #. DBT_REPOSITORY: A git repository URL to the DBT project
+    #. DBT_BRANCH: A git branch to use for the DBT project
+    #. DBT_REPOSITORY_PATH: A path to the DBT project in the git repository
+    #. EXTRA_DBT_PACKAGES: A list of python packages necessary for the DBT project
+    #. DBT_ENABLE_OVERRIDE: A boolean to enable/disable the DBT project override, those overrides
+       allows you to extend the DBT project without having to fork it. For this to work you need
+       to create a patch with the name ``dbt-packages`` and ``dbt-project``. We recommend to copy
+       the default DBT files (``dbt_project.yml`` and ``packages.yml``) and add your changes from
+       there.
+
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
```

### Comparing `tutor-contrib-aspects-0.4.0/README.rst` & `tutor-contrib-aspects-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: tutor-contrib-aspects
+Version: 0.5.0
+Summary: Aspects plugin for Tutor
+Home-page: https://github.com/open-craft/tutor-contrib-aspects
+Author: The Open edX Community
+License: AGPLv3
+Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
+Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+
 The Aspects plugin for Tutor
 ============================
 
 Aspects Learner Analytics combines several free, open source, tools to add analytics and reporting capabilities to the Open edX platform. This plugin offers easy installation, configuration, and deployment of these tools using `Tutor <https://docs.tutor.overhang.io>`__. The tools Aspects uses are:
 
 - `ClickHouse <https://clickhouse.com>`__, a fast, scalable analytics database that can be run anywhere
 - `Apache Superset <https://superset.apache.org>`__, a data visualization platform and data API
@@ -186,11 +207,27 @@
         "sk": {"flag": "sk", "name": "Slovak"},
         "sl": {"flag": "si", "name": "Slovenian"},
         "nl": {"flag": "nl", "name": "Dutch"},
     }
 
 Where the first key is the abbreviation of the language to use, "flag" is which flag icon is displayed in the user interface for choosing the language, and "name" is the displayed name for that language. The mapping above shows all of the current languages supported by Superset, but please note that different languages have different levels of completion and support at this time.
 
+
+Extending the DBT project
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+To extend the DBT project there are multiple options:
+
+    #. DBT_REPOSITORY: A git repository URL to the DBT project
+    #. DBT_BRANCH: A git branch to use for the DBT project
+    #. DBT_REPOSITORY_PATH: A path to the DBT project in the git repository
+    #. EXTRA_DBT_PACKAGES: A list of python packages necessary for the DBT project
+    #. DBT_ENABLE_OVERRIDE: A boolean to enable/disable the DBT project override, those overrides
+       allows you to extend the DBT project without having to fork it. For this to work you need
+       to create a patch with the name ``dbt-packages`` and ``dbt-project``. We recommend to copy
+       the default DBT files (``dbt_project.yml`` and ``packages.yml``) and add your changes from
+       there.
+
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
```

### Comparing `tutor-contrib-aspects-0.4.0/setup.py` & `tutor-contrib-aspects-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.4.0
+Version: 0.5.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -207,11 +207,27 @@
         "sk": {"flag": "sk", "name": "Slovak"},
         "sl": {"flag": "si", "name": "Slovenian"},
         "nl": {"flag": "nl", "name": "Dutch"},
     }
 
 Where the first key is the abbreviation of the language to use, "flag" is which flag icon is displayed in the user interface for choosing the language, and "name" is the displayed name for that language. The mapping above shows all of the current languages supported by Superset, but please note that different languages have different levels of completion and support at this time.
 
+
+Extending the DBT project
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+To extend the DBT project there are multiple options:
+
+    #. DBT_REPOSITORY: A git repository URL to the DBT project
+    #. DBT_BRANCH: A git branch to use for the DBT project
+    #. DBT_REPOSITORY_PATH: A path to the DBT project in the git repository
+    #. EXTRA_DBT_PACKAGES: A list of python packages necessary for the DBT project
+    #. DBT_ENABLE_OVERRIDE: A boolean to enable/disable the DBT project override, those overrides
+       allows you to extend the DBT project without having to fork it. For this to work you need
+       to create a patch with the name ``dbt-packages`` and ``dbt-project``. We recommend to copy
+       the default DBT files (``dbt_project.yml`` and ``packages.yml``) and add your changes from
+       there.
+
 License
 -------
 
 This software is licensed under the terms of the AGPLv3.
```

### Comparing `tutor-contrib-aspects-0.4.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 tutoraspects/patches/local-docker-compose-jobs-services
 tutoraspects/patches/local-docker-compose-services
 tutoraspects/patches/openedx-cms-common-settings
 tutoraspects/patches/superset-extra-assets
 tutoraspects/patches/superset-jinja-filters
 tutoraspects/templates/base-docker-compose-services
 tutoraspects/templates/aspects/apps/.gitignore
+tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
 tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
 tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
 tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
 tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
 tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
 tutoraspects/templates/aspects/apps/ralph/config/env
 tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
```

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,15 @@
         ("DBT_PROFILE_CUSTOM_SETTINGS", ""),
         # Allows the connection to understand the JSON type
         ("DBT_PROFILE_ALLOW_EXPERIMENTAL_OBJECT_TYPE", "True"),
         # Timeout for server ping
         ("DBT_PROFILE_SYNC_REQUEST_TIMEOUT", "5"),
         # Compression block size if compression is enabled, this is the default value
         ("DBT_PROFILE_COMPRESS_BLOCK_SIZE", "1048576"),
+        ("DBT_ENABLE_OVERRIDE", False),
     ]
 )
 
 # Ralph requires us to write out a file with pre-encrypted values, so we encrypt
 # them here per: https://openfun.github.io/ralph/api/#creating_a_credentials_file
 #
 # They will remain unchanged between config saves as usual and the unencryted
```

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.4.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.5.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

