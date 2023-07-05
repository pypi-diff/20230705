# Comparing `tmp/dockertown-0.2.2.tar.gz` & `tmp/dockertown-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockertown-0.2.2.tar", last modified: Thu Apr 20 23:16:30 2023, max compression
+gzip compressed data, was "dockertown-0.2.3.tar", last modified: Wed Jul  5 18:59:46 2023, max compression
```

## Comparing `dockertown-0.2.2.tar` & `dockertown-0.2.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.731968 dockertown-0.2.2/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2023-04-19 19:49:15.000000 dockertown-0.2.2/CONTRIBUTING.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2023-04-19 19:49:15.000000 dockertown-0.2.2/LICENSE
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       67 2023-04-19 19:49:15.000000 dockertown-0.2.2/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 23:16:30.731968 dockertown-0.2.2/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14262 2023-04-19 19:49:15.000000 dockertown-0.2.2/README.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.723967 dockertown-0.2.2/docs/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.723967 dockertown-0.2.2/docs/template/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4929 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_client.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/docs/template/docker_objects/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      692 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/builders.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/configs.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/containers.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/images.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/networks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      966 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/nodes.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/plugins.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/services.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      689 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/tasks.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/docker_objects/volumes.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/docs/template/sub-commands/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/sub-commands/buildx.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/sub-commands/compose.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1559 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/sub-commands/context.md
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/docs/template/user_guide/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/user_guide/docker_run.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      961 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/user_guide/exceptions.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/user_guide/generic_resources.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2023-04-19 19:49:15.000000 dockertown-0.2.2/docs/template/user_guide/running_inside_a_container.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:15.000000 dockertown-0.2.2/lint-requirements.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2023-04-20 15:09:42.000000 dockertown-0.2.2/requirements.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 23:16:30.731968 dockertown-0.2.2/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-04-20 23:16:29.000000 dockertown-0.2.2/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.723967 dockertown-0.2.2/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1332 2023-04-20 23:16:29.000000 dockertown-0.2.2/src/dockertown/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9429 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/client_config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/command_line_entrypoint.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/buildx/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    23517 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/buildx/imagetools/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/imagetools/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2892 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/imagetools/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/imagetools/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1016 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/buildx/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/compose/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/compose/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    31127 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/compose/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2918 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/compose/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/config/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/config/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/config/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      601 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/config/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/container/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/container/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    73220 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/container/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7450 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/container/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/context/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/context/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7724 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/context/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      542 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/context/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/image/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/image/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    26409 2023-04-20 21:59:14.000000 dockertown-0.2.2/src/dockertown/components/image/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2345 2023-04-20 23:02:24.000000 dockertown-0.2.2/src/dockertown/components/image/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/manifest/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/manifest/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5089 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/manifest/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      346 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/manifest/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/network/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/network/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/network/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/network/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/node/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/node/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/node/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2176 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/node/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/plugin/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/plugin/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/plugin/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      879 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/plugin/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/secret/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/secret/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/secret/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/secret/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/service/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/service/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/service/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/service/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/stack/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/stack/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/stack/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/swarm/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/swarm/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     9219 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/swarm/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown/components/system/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/system/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/system/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/system/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.731968 dockertown-0.2.2/src/dockertown/components/task/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/task/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/task/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/task/models.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.731968 dockertown-0.2.2/src/dockertown/components/trust/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/trust/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      486 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/trust/cli_wrapper.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.731968 dockertown-0.2.2/src/dockertown/components/volume/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/volume/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/volume/cli_wrapper.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      385 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/components/volume/models.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    12100 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/docker_client.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/download_binaries.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1807 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/py.typed
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      710 2023-04-19 19:49:15.000000 dockertown-0.2.2/src/dockertown/test_utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    11371 2023-04-20 23:02:24.000000 dockertown-0.2.2/src/dockertown/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.727968 dockertown-0.2.2/src/dockertown.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3882 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-04-20 23:16:30.000000 dockertown-0.2.2/src/dockertown.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 23:16:30.731968 dockertown-0.2.2/tests/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       29 2023-04-19 19:49:15.000000 dockertown-0.2.2/tests/test-requirements.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.733532 dockertown-0.2.3/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2475 2023-04-19 19:49:15.000000 dockertown-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1087 2023-04-19 19:49:15.000000 dockertown-0.2.3/LICENSE
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)       67 2023-04-19 19:49:15.000000 dockertown-0.2.3/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-07-05 18:59:46.729532 dockertown-0.2.3/PKG-INFO
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    14262 2023-04-19 19:49:15.000000 dockertown-0.2.3/README.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.721532 dockertown-0.2.3/docs/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/docs/template/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     4929 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_client.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/docs/template/docker_objects/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      692 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/builders.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1078 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/configs.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1042 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/containers.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1249 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/images.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1180 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/networks.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      966 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/nodes.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1037 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/plugins.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1108 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/services.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      689 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/tasks.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1103 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/docker_objects/volumes.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/docs/template/sub-commands/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1279 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/sub-commands/buildx.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2097 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/sub-commands/compose.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1559 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/sub-commands/context.md
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/docs/template/user_guide/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     3711 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/user_guide/docker_run.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      961 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/user_guide/exceptions.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     6442 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/user_guide/generic_resources.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     3364 2023-04-19 19:49:15.000000 dockertown-0.2.3/docs/template/user_guide/running_inside_a_container.md
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:15.000000 dockertown-0.2.3/lint-requirements.txt
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)       76 2023-07-05 18:53:46.000000 dockertown-0.2.3/requirements.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-07-05 18:59:46.733532 dockertown-0.2.3/setup.cfg
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1022 2023-07-05 18:55:32.000000 dockertown-0.2.3/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.721532 dockertown-0.2.3/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1332 2023-07-05 18:55:32.000000 dockertown-0.2.3/src/dockertown/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     9429 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/client_config.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1452 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/command_line_entrypoint.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown/components/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown/components/buildx/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    23517 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown/components/buildx/imagetools/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/imagetools/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2892 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/imagetools/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1364 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/imagetools/models.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1016 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/buildx/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown/components/compose/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/compose/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    31127 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/compose/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2918 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/compose/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/config/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/config/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     4775 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/config/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      601 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/config/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/container/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/container/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    73220 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/container/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     7450 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/container/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/context/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/context/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     7724 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/context/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      542 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/context/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/image/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/image/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    26409 2023-04-20 21:59:14.000000 dockertown-0.2.3/src/dockertown/components/image/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2345 2023-04-20 23:02:24.000000 dockertown-0.2.3/src/dockertown/components/image/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/manifest/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/manifest/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     5089 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/manifest/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      346 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/manifest/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/network/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/network/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     7548 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/network/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      820 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/network/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/node/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/node/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     7452 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/node/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2176 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/node/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/plugin/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/plugin/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     9428 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/plugin/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      879 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/plugin/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/secret/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/secret/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     3307 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/secret/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/secret/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/service/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/service/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    16688 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/service/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     2193 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/service/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/stack/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/stack/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     5523 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/stack/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/swarm/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/swarm/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     9219 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/swarm/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/system/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/system/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     6413 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/system/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     5429 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/system/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/task/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/task/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     3195 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/task/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     3811 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/task/models.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/trust/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/trust/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      486 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/trust/cli_wrapper.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/src/dockertown/components/volume/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/volume/__init__.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    10346 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/volume/cli_wrapper.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      385 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/components/volume/models.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    12100 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/docker_client.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     4364 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/download_binaries.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)     1807 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/exceptions.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)       69 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/py.typed
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      710 2023-04-19 19:49:15.000000 dockertown-0.2.3/src/dockertown/test_utils.py
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)    11384 2023-06-05 15:37:57.000000 dockertown-0.2.3/src/dockertown/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.725532 dockertown-0.2.3/src/dockertown.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    14716 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3882 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       72 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       76 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       11 2023-07-05 18:59:46.000000 dockertown-0.2.3/src/dockertown.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-07-05 18:59:46.729532 dockertown-0.2.3/tests/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)       29 2023-04-19 19:49:15.000000 dockertown-0.2.3/tests/test-requirements.txt
```

### Comparing `dockertown-0.2.2/CONTRIBUTING.md` & `dockertown-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/LICENSE` & `dockertown-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/PKG-INFO` & `dockertown-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockertown
-Version: 0.2.2
+Version: 0.2.3
 Summary: A decent Python wrapper for Docker CLI
 Home-page: UNKNOWN
 License: MIT
 Project-URL: Documentation, https://duckietown.github.io/dockertown/
 Project-URL: Source Code, https://github.com/duckietown/dockertown
 Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
 Platform: UNKNOWN
```

### Comparing `dockertown-0.2.2/README.md` & `dockertown-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_client.md` & `dockertown-0.2.3/docs/template/docker_client.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/builders.md` & `dockertown-0.2.3/docs/template/docker_objects/builders.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/configs.md` & `dockertown-0.2.3/docs/template/docker_objects/configs.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/containers.md` & `dockertown-0.2.3/docs/template/docker_objects/containers.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/images.md` & `dockertown-0.2.3/docs/template/docker_objects/images.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/networks.md` & `dockertown-0.2.3/docs/template/docker_objects/networks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/nodes.md` & `dockertown-0.2.3/docs/template/docker_objects/nodes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/plugins.md` & `dockertown-0.2.3/docs/template/docker_objects/plugins.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/services.md` & `dockertown-0.2.3/docs/template/docker_objects/services.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/tasks.md` & `dockertown-0.2.3/docs/template/docker_objects/tasks.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/docker_objects/volumes.md` & `dockertown-0.2.3/docs/template/docker_objects/volumes.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/sub-commands/buildx.md` & `dockertown-0.2.3/docs/template/sub-commands/buildx.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/sub-commands/compose.md` & `dockertown-0.2.3/docs/template/sub-commands/compose.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/sub-commands/context.md` & `dockertown-0.2.3/docs/template/sub-commands/context.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/user_guide/docker_run.md` & `dockertown-0.2.3/docs/template/user_guide/docker_run.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/user_guide/exceptions.md` & `dockertown-0.2.3/docs/template/user_guide/exceptions.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/user_guide/generic_resources.md` & `dockertown-0.2.3/docs/template/user_guide/generic_resources.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/docs/template/user_guide/running_inside_a_container.md` & `dockertown-0.2.3/docs/template/user_guide/running_inside_a_container.md`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/setup.py` & `dockertown-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_long_description() -> str:
     return (CURRENT_DIR / "README.md").read_text(encoding="utf8")
 
 
 setup(
     name="dockertown",
-    version="0.2.2",
+    version="0.2.3",
     description="A decent Python wrapper for Docker CLI",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     install_requires=(CURRENT_DIR / "requirements.txt").read_text().splitlines(),
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,  # will read the MANIFEST.in
```

### Comparing `dockertown-0.2.2/src/dockertown/__init__.py` & `dockertown-0.2.3/src/dockertown/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from .client_config import ClientNotFoundError
 from .components.buildx.cli_wrapper import Builder
 from .components.config.cli_wrapper import Config
 from .components.container.cli_wrapper import Container, ContainerStats
 from .components.context.cli_wrapper import (
     Context,
```

### Comparing `dockertown-0.2.2/src/dockertown/client_config.py` & `dockertown-0.2.3/src/dockertown/client_config.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/command_line_entrypoint.py` & `dockertown-0.2.3/src/dockertown/command_line_entrypoint.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/buildx/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/buildx/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/buildx/imagetools/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/buildx/imagetools/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/buildx/imagetools/models.py` & `dockertown-0.2.3/src/dockertown/components/buildx/imagetools/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/buildx/models.py` & `dockertown-0.2.3/src/dockertown/components/buildx/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/compose/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/compose/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/compose/models.py` & `dockertown-0.2.3/src/dockertown/components/compose/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/config/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/config/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/config/models.py` & `dockertown-0.2.3/src/dockertown/components/config/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/container/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/container/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/container/models.py` & `dockertown-0.2.3/src/dockertown/components/container/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/context/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/context/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/context/models.py` & `dockertown-0.2.3/src/dockertown/components/context/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/image/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/image/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/image/models.py` & `dockertown-0.2.3/src/dockertown/components/image/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/manifest/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/manifest/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/network/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/network/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/network/models.py` & `dockertown-0.2.3/src/dockertown/components/network/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/node/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/node/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/node/models.py` & `dockertown-0.2.3/src/dockertown/components/node/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/plugin/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/plugin/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/plugin/models.py` & `dockertown-0.2.3/src/dockertown/components/plugin/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/secret/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/secret/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/service/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/service/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/service/models.py` & `dockertown-0.2.3/src/dockertown/components/service/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/stack/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/stack/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/swarm/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/swarm/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/system/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/system/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/system/models.py` & `dockertown-0.2.3/src/dockertown/components/system/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/task/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/task/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/task/models.py` & `dockertown-0.2.3/src/dockertown/components/task/models.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/components/volume/cli_wrapper.py` & `dockertown-0.2.3/src/dockertown/components/volume/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/docker_client.py` & `dockertown-0.2.3/src/dockertown/docker_client.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/download_binaries.py` & `dockertown-0.2.3/src/dockertown/download_binaries.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/exceptions.py` & `dockertown-0.2.3/src/dockertown/exceptions.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/test_utils.py` & `dockertown-0.2.3/src/dockertown/test_utils.py`

 * *Files identical despite different names*

### Comparing `dockertown-0.2.2/src/dockertown/utils.py` & `dockertown-0.2.3/src/dockertown/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
                 full_stderr += line
 
     exit_code = process.wait()
     if exit_code != 0:
         raise DockerException(full_cmd, exit_code, stderr=full_stderr)
 
 
-def format_dict_for_cli(dictionary: Dict[str, str], separator="="):
+def format_dict_for_cli(dictionary: Dict[str, str], separator="=") -> List[str]:
     return [f"{key}{separator}{value}" for key, value in dictionary.items()]
 
 
 def read_env_file(env_file: Path) -> Dict[str, str]:
     result_dict = {}
     for line in env_file.read_text().splitlines():
         line = line.strip()
```

### Comparing `dockertown-0.2.2/src/dockertown.egg-info/PKG-INFO` & `dockertown-0.2.3/src/dockertown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockertown
-Version: 0.2.2
+Version: 0.2.3
 Summary: A decent Python wrapper for Docker CLI
 Home-page: UNKNOWN
 License: MIT
 Project-URL: Documentation, https://duckietown.github.io/dockertown/
 Project-URL: Source Code, https://github.com/duckietown/dockertown
 Project-URL: Bug Tracker, https://github.com/duckietown/dockertown/issues
 Platform: UNKNOWN
```

### Comparing `dockertown-0.2.2/src/dockertown.egg-info/SOURCES.txt` & `dockertown-0.2.3/src/dockertown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

