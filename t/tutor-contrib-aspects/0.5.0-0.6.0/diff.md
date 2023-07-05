# Comparing `tmp/tutor-contrib-aspects-0.5.0.tar.gz` & `tmp/tutor-contrib-aspects-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.5.0.tar", last modified: Wed Jul  5 16:47:54 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.6.0.tar", last modified: Wed Jul  5 19:40:56 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.5.0.tar` & `tutor-contrib-aspects-0.6.0.tar`

### file list

```diff
@@ -1,93 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 16:47:54.000000 tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.285130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    23845 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.281130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:47:54.289130 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 16:47:46.000000 tutor-contrib-aspects-0.5.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.056069 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 19:40:56.000000 tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.056069 tutor-contrib-aspects-0.6.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.056069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.052069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.052069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.052069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.060069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    41177 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.056069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/dbt/init-dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:40:56.064069 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 19:40:48.000000 tutor-contrib-aspects-0.6.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.5.0/PKG-INFO` & `tutor-contrib-aspects-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.5.0
+Version: 0.6.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.5.0/README.rst` & `tutor-contrib-aspects-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/setup.py` & `tutor-contrib-aspects-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.5.0
+Version: 0.6.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.5.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.6.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
 tutoraspects/templates/aspects/apps/superset/security/roles.json
 tutoraspects/templates/aspects/apps/vector/file.toml
 tutoraspects/templates/aspects/apps/vector/k8s.toml
 tutoraspects/templates/aspects/apps/vector/local.toml
 tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
 tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
 tutoraspects/templates/aspects/build/.gitignore
```

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.6.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.5.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.6.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

