# Comparing `tmp/anycluster-2.3.3.tar.gz` & `tmp/anycluster-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.3.3.tar", last modified: Wed Jun 14 09:36:24 2023, max compression
+gzip compressed data, was "anycluster-2.3.4.tar", last modified: Wed Jul  5 15:28:04 2023, max compression
```

## Comparing `anycluster-2.3.3.tar` & `anycluster-2.3.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.664059 anycluster-2.3.3/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.3/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.3/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-14 09:36:24.660060 anycluster-2.3.3/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.3/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.3/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3536 2023-06-13 06:05:24.000000 anycluster-2.3.3/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    38351 2023-06-13 06:57:30.000000 anycluster-2.3.3/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.3/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.3/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.3/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.3/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     4685 2023-06-13 06:41:38.000000 anycluster-2.3.3/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.3/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     8087 2023-06-12 13:31:27.000000 anycluster-2.3.3/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.3/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5293 2023-06-13 06:41:37.000000 anycluster-2.3.3/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.656060 anycluster-2.3.3/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.3/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.3.3/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.3/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.3/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10055 2023-06-12 13:28:29.000000 anycluster-2.3.3/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.3/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.3/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.3/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.660060 anycluster-2.3.3/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.3/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.3/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    16491 2023-06-13 07:05:25.000000 anycluster-2.3.3/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.3/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.3/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.3/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.3/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    28275 2023-06-13 07:05:23.000000 anycluster-2.3.3/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.3/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-14 09:36:24.652060 anycluster-2.3.3/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-14 09:36:24.000000 anycluster-2.3.3/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-14 09:36:24.664059 anycluster-2.3.3/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-14 09:36:13.000000 anycluster-2.3.3/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.568175 anycluster-2.3.4/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.4/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.4/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-07-05 15:28:04.568175 anycluster-2.3.4/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.4/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.4/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3606 2023-07-05 14:36:07.000000 anycluster-2.3.4/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    38993 2023-07-05 14:40:12.000000 anycluster-2.3.4/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.4/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.4/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.4/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.4/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     4685 2023-06-13 06:41:38.000000 anycluster-2.3.4/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.4/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     8087 2023-06-12 13:31:27.000000 anycluster-2.3.4/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.4/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5293 2023-06-13 06:41:37.000000 anycluster-2.3.4/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.4/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2829 2023-06-13 06:32:28.000000 anycluster-2.3.4/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.4/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3519 2023-06-13 06:32:18.000000 anycluster-2.3.4/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.4/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.4/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10055 2023-06-12 13:28:29.000000 anycluster-2.3.4/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.4/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.4/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.560175 anycluster-2.3.4/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.560175 anycluster-2.3.4/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.568175 anycluster-2.3.4/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.4/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.568175 anycluster-2.3.4/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.568175 anycluster-2.3.4/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.4/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.4/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.4/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.4/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.4/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    17417 2023-07-05 15:21:13.000000 anycluster-2.3.4/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.4/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.4/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.4/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.4/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    30464 2023-07-05 15:21:06.000000 anycluster-2.3.4/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.4/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-07-05 15:28:04.564175 anycluster-2.3.4/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-07-05 15:28:04.000000 anycluster-2.3.4/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-07-05 15:28:04.000000 anycluster-2.3.4/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-07-05 15:28:04.000000 anycluster-2.3.4/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-07-05 15:28:04.000000 anycluster-2.3.4/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-07-05 15:28:04.000000 anycluster-2.3.4/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-07-05 15:28:04.568175 anycluster-2.3.4/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-07-05 15:27:32.000000 anycluster-2.3.4/setup.py
```

### Comparing `anycluster-2.3.3/LICENSE` & `anycluster-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/PKG-INFO` & `anycluster-2.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.3
+Version: 2.3.4
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.3/README.md` & `anycluster-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/ClusterCache.py` & `anycluster-2.3.4/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/FilterComposer.py` & `anycluster-2.3.4/anycluster/FilterComposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,19 @@
         
         if len(filters) > 1:
             filterstring += ')'
 
         return filterstring
 
 
-    def as_sql(self):
+    def as_sql(self, omit_leading_AND=False):
 
         filterstring = ''
 
         if self.filters:
 
-            filterstring = ' AND '
+            if omit_leading_AND == False:
+                filterstring = ' AND '
 
             filterstring += self.parse_filters(self.filters)
 
         return filterstring
```

### Comparing `anycluster-2.3.3/anycluster/MapClusterer.py` & `anycluster-2.3.4/anycluster/MapClusterer.py`

 * *Files 3% similar despite different names*

```diff
@@ -790,49 +790,62 @@
         # currently, the geometry type for counting is always set to GEOMETRY_TYPE_AREA,
         # because otherwise pins which are outside the current viewport, but inside the cluster geometry would be counted
         # the pins visible on the map would not always be the returned count if GEOMETRY_TYPE_VIEWPORT was supported
         geometry_type = GEOMETRY_TYPE_AREA
 
         geometries_for_counting = self.get_geometries_for_counting(geojson, geometry_type, zoom)
 
-        unmodulated_count = self.query_map_content_count(geometries_for_counting, filters)
+        unmodulated_count = self.query_map_content_count(geometries_for_counting, filters, [])
         result['count'] = unmodulated_count
 
         for modulation_name, modulation_filters in modulations.items():
 
             if 'filters' in modulation_filters:
-                combined_filters = filters + modulation_filters['filters']
+                modulation_filters = modulation_filters['filters']
             else:
-                combined_filters = filters + [modulation_filters]
+                modulation_filters = [modulation_filters]
                 
-            modulated_count = self.query_map_content_count(geometries_for_counting, combined_filters)
+            modulated_count = self.query_map_content_count(geometries_for_counting, filters, modulation_filters)
             result['modulations'][modulation_name] = {
                 'count': modulated_count
             }
 
         return result
 
 
-    def query_map_content_count(self, geometries_for_counting, filters):
+    # a nested select is required for the modulation filters
+    def query_map_content_count(self, geometries_for_counting, filters, modulation_filters):
 
         count = 0
 
         filter_composer = FilterComposer(filters)
         filterstring = filter_composer.as_sql()
 
         geom_filterstring = self.get_geom_filter_string_from_geos(geometries_for_counting)
 
+        modulation_filter_composer = FilterComposer(modulation_filters)
+        modulation_filterstring = modulation_filter_composer.as_sql(omit_leading_AND=True)
+
         content_count_sql = '''
-            SELECT count(*) AS count
-            FROM {schema_name}.{geo_table}
-                WHERE {geo_column_str} IS NOT NULL
-                    AND {geom_filterstring} {filterstring};
+            SELECT count(*) AS count FROM
+                (SELECT * FROM {schema_name}.{geo_table}
+                    WHERE {geo_column_str} IS NOT NULL
+                        AND {geom_filterstring} {filterstring}
+                ) AS markers
         '''.format(schema_name=self.schema_name, geo_table=geo_table, geo_column_str=geo_column_str,
                     geom_filterstring=geom_filterstring, filterstring=filterstring)
 
+        if modulation_filterstring:
+            content_count_sql = '{content_count_sql} WHERE {modulation_filterstring}'.format(
+                content_count_sql=content_count_sql, modulation_filterstring=modulation_filterstring
+            )
+
+
+        content_count_sql = '{content_count_sql};'.format(content_count_sql=content_count_sql)
+
         cursor = connections['default'].cursor()
         cursor.execute(content_count_sql)
         query_result = cursor.fetchone()
 
         count += query_result[0]
 
         return count
```

### Comparing `anycluster-2.3.3/anycluster/MapTools.py` & `anycluster-2.3.4/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/json_schemas.py` & `anycluster-2.3.4/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/serializers.py` & `anycluster-2.3.4/anycluster/api/serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.3.4/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/tests/test_serializers.py` & `anycluster-2.3.4/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/tests/test_views.py` & `anycluster-2.3.4/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/urls.py` & `anycluster-2.3.4/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/api/views.py` & `anycluster-2.3.4/anycluster/api/views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/clusters.py` & `anycluster-2.3.4/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/definitions.py` & `anycluster-2.3.4/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/globalmaptiles.py` & `anycluster-2.3.4/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/10.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/100.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/1000.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/10000.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/5.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/50.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.3.4/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.3.4/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 13 07:05:23 2023 UTC, .py size: 28275 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 3315 8864 736e 0000  U.......3..dsn..
+00000000: 550d 0d0a 0000 0000 628a a564 0077 0000  U.......b..d.w..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
@@ -648,384 +648,442 @@
 00002870: 0000 0072 7b00 0000 727c 0000 0072 7d00  ...r{...r|...r}.
 00002880: 0000 722e 0000 0072 2e00 0000 722e 0000  ..r....r....r...
 00002890: 0072 2f00 0000 721b 0000 0014 0000 0073  .r/...r........s
 000028a0: 2c00 0000 0803 0815 0812 0822 0816 0813  ,.........."....
 000028b0: 0817 0825 0817 0815 0813 0816 0815 0826  ...%...........&
 000028c0: 0817 0818 081b 0820 0813 0803 0803 0803  ....... ........
 000028d0: 721b 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000028e0: 0000 0000 0000 0200 0000 4000 0000 7334  ..........@...s4
+000028e0: 0000 0000 0000 0200 0000 4000 0000 733c  ..........@...s<
 000028f0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
 00002900: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
 00002910: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
-00002920: 005a 0764 0b53 0029 0cda 1d54 6573 744d  .Z.d.S.)...TestM
-00002930: 6170 436c 7573 7465 7265 7243 6f6e 7465  apClustererConte
-00002940: 6e74 436f 756e 7473 6301 0000 0000 0000  ntCountsc.......
-00002950: 0000 0000 000f 0000 000a 0000 0043 0000  .............C..
-00002960: 0073 cc01 0000 6401 7d01 6402 6403 6404  .s....d.}.d.d.d.
-00002970: 6405 9c03 6701 7d02 6406 6407 6408 6404  d...g.}.d.d.d.d.
-00002980: 6405 9c03 6701 6901 6406 6407 6408 6409  d...g.i.d.d.d.d.
-00002990: 6405 9c03 6701 6901 640a 9c02 7d03 6407  d...g.i.d...}.d.
-000029a0: 6408 6404 6405 9c03 6407 6408 6409 6405  d.d.d...d.d.d.d.
-000029b0: 9c03 640a 9c02 7d04 7400 4400 9001 5d6e  ..d...}.t.D...]n
-000029c0: 7d05 7401 4400 9001 5d62 7d06 7402 7403  }.t.D...]b}.t.t.
-000029d0: 7404 7405 6604 4400 9001 5d4e 7d07 7c05  t.t.f.D...]N}.|.
-000029e0: 7406 6b02 728a 7c06 7407 6b03 728a 7172  t.k.r.|.t.k.r.qr
-000029f0: 7c06 7407 6b02 729c 7c07 7403 6b03 729c  |.t.k.r.|.t.k.r.
-00002a00: 7172 7c00 a008 7c06 7c01 7c05 7c02 a104  qr|...|.|.|.|...
-00002a10: 7d08 7409 7c08 740a 640b 8d02 7d09 7c09  }.t.|.t.d...}.|.
-00002a20: a00b 7c07 7c06 7c02 7c01 7c03 a105 7d0a  ..|.|.|.|.|...}.
-00002a30: 7c09 a00b 7c07 7c06 7c02 7c01 7c04 a105  |...|.|.|.|.|...
-00002a40: 0400 7d0b 7d0a 640c 640d 640c 6901 640d  ..}.}.d.d.d.i.d.
-00002a50: 640c 6901 640a 9c02 640e 9c02 7d0c 7c00  d.i.d...d...}.|.
-00002a60: a00c 7c0a 7c0c a102 0100 7c00 a00c 7c0b  ..|.|.....|...|.
-00002a70: 7c0c a102 0100 7c06 7407 6b02 9001 728a  |.....|.t.k...r.
-00002a80: 7c00 a00d 640f 6403 a102 0100 7c00 a00d  |...d.d.....|...
-00002a90: 6410 6411 a102 0100 7c09 a00b 7c07 7c06  d.d.....|...|.|.
-00002aa0: 7c02 7c01 7c03 a105 7d0a 7c09 a00b 7c07  |.|.|...}.|...|.
-00002ab0: 7c06 7c02 7c01 7c04 a105 0400 7d0b 7d0a  |.|.|.|.....}.}.
-00002ac0: 6412 640d 640c 6901 640d 6412 6901 640a  d.d.d.i.d.d.i.d.
-00002ad0: 9c02 640e 9c02 7d0c 7c00 a00c 7c0a 7c0c  ..d...}.|...|.|.
-00002ae0: a102 0100 7c00 a00c 7c0b 7c0c a102 0100  ....|...|.|.....
-00002af0: 740e 6a0f a010 a100 7d0d 7c0d 4400 5d0e  t.j.....}.|.D.].
-00002b00: 7d0e 7c0e a011 a100 0100 9001 7198 740e  }.|.........q.t.
-00002b10: 6a0f a010 a100 7d0d 7c00 a00c 7c0d a012  j.....}.|...|...
-00002b20: a100 640c a102 0100 7172 7160 7156 6400  ..d.....qrq`qVd.
-00002b30: 5300 2913 4e72 6a00 0000 7254 0000 00da  S.).Nrj...rT....
-00002b40: 0573 746f 6e65 fa01 3da9 03da 0663 6f6c  .stone..=....col
-00002b50: 756d 6eda 0576 616c 7565 da08 6f70 6572  umn..value..oper
-00002b60: 6174 6f72 722b 0000 0072 5600 0000 547a  atorr+...rV...Tz
-00002b70: 0221 3d29 02da 0466 7265 655a 0470 6169  .!=)...freeZ.pai
-00002b80: 64a9 0172 2500 0000 7201 0000 0072 6100  d..r%...r....ra.
-00002b90: 0000 2902 7261 0000 00da 0b6d 6f64 756c  ..).ra.....modul
-00002ba0: 6174 696f 6e73 fa06 6e61 6d65 2031 fa06  ations..name 1..
-00002bb0: 6e61 6d65 2032 da06 666c 6f77 6572 7231  name 2..flowerr1
-00002bc0: 0000 0029 1372 0b00 0000 720e 0000 0072  ...).r....r....r
-00002bd0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00002be0: 0000 0072 1000 0000 720c 0000 0072 2000  ...r....r....r .
-00002bf0: 0000 7209 0000 00da 0e54 4553 545f 4752  ..r......TEST_GR
-00002c00: 4944 5f53 495a 455a 1667 6574 5f6d 6170  ID_SIZEZ.get_map
-00002c10: 5f63 6f6e 7465 6e74 5f63 6f75 6e74 7372  _content_countsr
-00002c20: 2100 0000 da0c 6372 6561 7465 5f70 6f69  !.....create_poi
-00002c30: 6e74 7218 0000 0072 7200 0000 7273 0000  ntr....rr...rs..
-00002c40: 00da 0664 656c 6574 6572 6100 0000 290f  ...deletera...).
-00002c50: 7227 0000 0072 2c00 0000 722b 0000 0072  r'...r,...r+...r
-00002c60: 8a00 0000 5a12 7369 6d70 6c65 5f6d 6f64  ....Z.simple_mod
-00002c70: 756c 6174 696f 6e73 7228 0000 0072 2900  ulationsr(...r).
-00002c80: 0000 7238 0000 0072 2200 0000 722d 0000  ..r8...r"...r-..
-00002c90: 00da 0672 6573 756c 745a 1e72 6573 756c  ...resultZ.resul
-00002ca0: 745f 6672 6f6d 5f73 696d 706c 655f 6d6f  t_from_simple_mo
-00002cb0: 6475 6c61 7469 6f6e 73da 0f65 7870 6563  dulations..expec
-00002cc0: 7465 645f 7265 7375 6c74 da07 6761 7264  ted_result..gard
-00002cd0: 656e 7372 7600 0000 722e 0000 0072 2e00  ensrv...r....r..
-00002ce0: 0000 722f 0000 00da 1b74 6573 745f 6765  ..r/.....test_ge
-00002cf0: 745f 6d61 705f 636f 6e74 656e 745f 636f  t_map_content_co
-00002d00: 756e 7473 e201 0000 73a6 0000 0000 0204  unts....s.......
-00002d10: 0502 0102 0102 fd04 ff04 0b02 0202 0102  ................
-00002d20: 0102 fd04 ff02 fe02 0b02 0202 0102 0102  ................
-00002d30: fd04 ff02 ff02 f506 1802 0102 0102 fd04  ................
-00002d40: 0602 0102 0102 fd04 fa06 0e0a 010a 0212  ................
-00002d50: 0210 0102 0210 0102 0210 010c 0212 0206  ................
-00002d60: 0102 0002 0002 0002 ff08 0402 0302 0002  ................
-00002d70: ff02 0402 0002 ff02 fc04 fe06 0b0c 010c  ................
-00002d80: 020a 020c 010c 0212 0106 0102 0002 0002  ................
-00002d90: 0002 ff08 0402 0302 0002 ff02 0402 0002  ................
-00002da0: ff02 fc04 fe06 0e0c 010c 020a 0108 010c  ................
-00002db0: 030a 027a 3954 6573 744d 6170 436c 7573  ...z9TestMapClus
-00002dc0: 7465 7265 7243 6f6e 7465 6e74 436f 756e  tererContentCoun
-00002dd0: 7473 2e74 6573 745f 6765 745f 6d61 705f  ts.test_get_map_
-00002de0: 636f 6e74 656e 745f 636f 756e 7473 6301  content_countsc.
-00002df0: 0000 0000 0000 0000 0000 000c 0000 0006  ................
-00002e00: 0000 0043 0000 0073 3201 0000 6401 7d01  ...C...s2...d.}.
-00002e10: 7400 7d02 7401 7d03 6700 7d04 7c00 a002  t.}.t.}.g.}.|...
-00002e20: 7c02 7c01 7c03 7c04 a104 7d05 7403 7c05  |.|.|.|...}.t.|.
-00002e30: 7404 6402 8d02 7d06 7405 7d07 7c06 a006  t.d...}.t.}.|...
-00002e40: 7c07 7c02 7c01 a103 7d08 7c06 a007 7c08  |.|.|...}.|...|.
-00002e50: 7c04 a102 7d09 7c00 a008 7c09 6403 a102  |...}.|...|.d...
-00002e60: 0100 7c00 a009 6404 6405 a102 0100 7c06  ..|...d.d.....|.
-00002e70: a007 7c08 7c04 a102 7d09 7c00 a008 7c09  ..|.|...}.|...|.
-00002e80: 6406 a102 0100 7c00 a009 6407 6408 a102  d.....|...d.d...
-00002e90: 0100 7c06 a007 7c08 7c04 a102 7d09 7c00  ..|...|.|...}.|.
-00002ea0: a008 7c09 6409 a102 0100 640a 6405 640b  ..|.d.....d.d.d.
-00002eb0: 640c 9c03 6701 7d04 7c06 a007 7c08 7c04  d...g.}.|...|.|.
-00002ec0: a102 7d09 7c00 a008 7c09 6406 a102 0100  ..}.|...|.d.....
-00002ed0: 640a 6405 640b 640c 9c03 640a 6408 640b  d.d.d.d...d.d.d.
-00002ee0: 640d 640e 9c04 6702 7d04 7c06 a007 7c08  d.d...g.}.|...|.
-00002ef0: 7c04 a102 7d09 7c00 a008 7c09 6409 a102  |...}.|...|.d...
-00002f00: 0100 740a 6a0b a00c a100 7d0a 7c0a 4400  ..t.j.....}.|.D.
-00002f10: 5d0e 7d0b 7c0b a00d a100 0100 9001 7104  ].}.|.........q.
-00002f20: 740a 6a0b a00c a100 7d0a 7c00 a008 7c0a  t.j.....}.|...|.
-00002f30: a00e a100 6403 a102 0100 6400 5300 290f  ....d.....d.S.).
-00002f40: 4e72 6a00 0000 7289 0000 0072 0100 0000  Nrj...r....r....
-00002f50: 728b 0000 0072 8200 0000 7231 0000 0072  r....r....r1...r
-00002f60: 8c00 0000 728d 0000 0072 3300 0000 7254  ....r....r3...rT
-00002f70: 0000 0072 8300 0000 7284 0000 00da 024f  ...r....r......O
-00002f80: 5229 0472 8500 0000 7286 0000 0072 8700  R).r....r....r..
-00002f90: 0000 da0f 6c6f 6769 6361 6c4f 7065 7261  ....logicalOpera
-00002fa0: 746f 7229 0f72 0c00 0000 720f 0000 0072  tor).r....r....r
-00002fb0: 2000 0000 7209 0000 0072 8e00 0000 7212   ...r....r....r.
-00002fc0: 0000 00da 1b67 6574 5f67 656f 6d65 7472  .....get_geometr
-00002fd0: 6965 735f 666f 725f 636f 756e 7469 6e67  ies_for_counting
-00002fe0: 5a17 7175 6572 795f 6d61 705f 636f 6e74  Z.query_map_cont
-00002ff0: 656e 745f 636f 756e 7472 2100 0000 728f  ent_countr!...r.
-00003000: 0000 0072 1800 0000 7272 0000 0072 7300  ...r....rr...rs.
-00003010: 0000 7290 0000 0072 6100 0000 290c 7227  ..r....ra...).r'
-00003020: 0000 0072 2c00 0000 7229 0000 0072 2800  ...r,...r)...r(.
-00003030: 0000 722b 0000 0072 2200 0000 722d 0000  ..r+...r"...r-..
-00003040: 0072 3800 0000 5a17 6765 6f6d 6574 7269  .r8...Z.geometri
-00003050: 6573 5f66 6f72 5f63 6f75 6e74 696e 6772  es_for_countingr
-00003060: 6100 0000 7293 0000 0072 7600 0000 722e  a...r....rv...r.
-00003070: 0000 0072 2e00 0000 722f 0000 00da 1c74  ...r....r/.....t
-00003080: 6573 745f 7175 6572 795f 6d61 705f 636f  est_query_map_co
-00003090: 6e74 656e 745f 636f 756e 7458 0200 0073  ntent_countX...s
-000030a0: 5000 0000 0002 0401 0401 0403 0402 1001  P...............
-000030b0: 0c02 0402 0e02 0c01 0c02 0c02 0c01 0c02  ................
-000030c0: 0c02 0c01 0c05 0201 0201 02fd 04ff 0408  ................
-000030d0: 0c01 0c04 0201 0201 02fd 0406 0201 0201  ................
-000030e0: 0201 02fc 04fa 040e 0c01 0c02 0a01 0801  ................
-000030f0: 0c03 0a02 7a3a 5465 7374 4d61 7043 6c75  ....z:TestMapClu
-00003100: 7374 6572 6572 436f 6e74 656e 7443 6f75  stererContentCou
-00003110: 6e74 732e 7465 7374 5f71 7565 7279 5f6d  nts.test_query_m
-00003120: 6170 5f63 6f6e 7465 6e74 5f63 6f75 6e74  ap_content_count
-00003130: 6301 0000 0000 0000 0000 0000 000a 0000  c...............
-00003140: 0009 0000 0043 0000 0073 aa00 0000 6401  .....C...s....d.
-00003150: 7d01 7400 4400 5d9c 7d02 7401 4400 5d92  }.t.D.].}.t.D.].
-00003160: 7d03 7402 7403 7404 7405 6604 4400 5d80  }.t.t.t.t.f.D.].
-00003170: 7d04 7c02 7406 6b02 7236 7c03 7407 6b03  }.|.t.k.r6|.t.k.
-00003180: 7236 7120 7c03 7407 6b02 7248 7c04 7403  r6q |.t.k.rH|.t.
-00003190: 6b03 7248 7120 6700 7d05 7c00 a008 7c03  k.rHq g.}.|...|.
-000031a0: 7c01 7c02 7c05 a104 7d06 7409 7c06 740a  |.|.|...}.t.|.t.
-000031b0: 6402 8d02 7d07 7c07 a00b 7c04 7c03 7c01  d...}.|...|.|.|.
-000031c0: a103 7d08 7c00 a00c 740d 7c08 740e 8302  ..}.|...t.|.t...
-000031d0: a101 0100 7c08 4400 5d14 7d09 7c00 a00c  ....|.D.].}.|...
-000031e0: 6403 7c09 6a0f 6b06 a101 0100 718a 7120  d.|.j.k.....q.q 
-000031f0: 7110 7108 6400 5300 2904 4e72 6a00 0000  q.q.d.S.).Nrj...
-00003200: 7289 0000 00da 0750 4f4c 5947 4f4e 2910  r......POLYGON).
-00003210: 720b 0000 0072 0e00 0000 7211 0000 0072  r....r....r....r
-00003220: 1200 0000 7213 0000 0072 1400 0000 7210  ....r....r....r.
-00003230: 0000 0072 0c00 0000 7220 0000 0072 0900  ...r....r ...r..
-00003240: 0000 728e 0000 0072 9700 0000 7235 0000  ..r....r....r5..
-00003250: 0072 3600 0000 7263 0000 00da 0377 6b74  .r6...rc.....wkt
-00003260: 290a 7227 0000 0072 2c00 0000 7228 0000  ).r'...r,...r(..
-00003270: 0072 2900 0000 7238 0000 0072 2b00 0000  .r)...r8...r+...
-00003280: 7222 0000 0072 2d00 0000 7239 0000 0072  r"...r-...r9...r
-00003290: 4300 0000 722e 0000 0072 2e00 0000 722f  C...r....r....r/
-000032a0: 0000 00da 2074 6573 745f 6765 745f 6765  .... test_get_ge
-000032b0: 6f6d 6574 7269 6573 5f66 6f72 5f63 6f75  ometries_for_cou
-000032c0: 6e74 696e 679c 0200 0073 1e00 0000 0002  nting....s......
-000032d0: 0402 0801 0802 1002 1001 0202 1001 0202  ................
-000032e0: 0402 1001 0c02 0e02 1002 0802 7a3e 5465  ............z>Te
-000032f0: 7374 4d61 7043 6c75 7374 6572 6572 436f  stMapClustererCo
-00003300: 6e74 656e 7443 6f75 6e74 732e 7465 7374  ntentCounts.test
-00003310: 5f67 6574 5f67 656f 6d65 7472 6965 735f  _get_geometries_
-00003320: 666f 725f 636f 756e 7469 6e67 6301 0000  for_countingc...
-00003330: 0000 0000 0000 0000 000a 0000 0008 0000  ................
-00003340: 0043 0000 0073 8e00 0000 6700 7d01 6401  .C...s....g.}.d.
-00003350: 7d02 7400 4400 5d7c 7d03 7401 4400 5d72  }.t.D.]|}.t.D.]r
-00003360: 7d04 7c00 a002 7c04 7c02 7c03 7c01 a104  }.|...|.|.|.|...
-00003370: 7d05 7403 7c05 7404 6402 8d02 7d06 7c06  }.t.|.t.d...}.|.
-00003380: a005 7406 a101 7d07 7c06 a007 7c07 7c02  ..t...}.|...|.|.
-00003390: a102 7d08 7c00 a008 7409 7c08 8301 6403  ..}.|...t.|...d.
-000033a0: a102 0100 7c00 a008 7c08 6a0a 6404 a102  ....|...|.j.d...
-000033b0: 0100 7c08 a00b 6405 a101 0100 6406 7d09  ..|...d.....d.}.
-000033c0: 7c00 a008 7c09 7409 7c08 8301 a102 0100  |...|.t.|.......
-000033d0: 7114 710c 6400 5300 2907 4e72 6a00 0000  q.q.d.S.).Nrj...
-000033e0: 7289 0000 007a a753 5249 443d 3338 3537  r....z.SRID=3857
-000033f0: 3b50 4f4c 5947 4f4e 2028 2839 3738 3339  ;POLYGON ((97839
-00003400: 332e 3936 3230 3520 3539 3438 3633 352e  3.96205 5948635.
-00003410: 3238 3930 3136 2c20 3135 3635 3433 302e  289016, 1565430.
-00003420: 3333 3932 3820 3539 3438 3633 352e 3238  33928 5948635.28
-00003430: 3930 3136 2c20 3135 3635 3433 302e 3333  9016, 1565430.33
-00003440: 3932 3820 3635 3734 3830 372e 3432 3437  928 6574807.4247
-00003450: 3238 2c20 3937 3833 3933 2e39 3632 3035  28, 978393.96205
-00003460: 2036 3537 3438 3037 2e34 3234 3732 382c   6574807.424728,
-00003470: 2039 3738 3339 332e 3936 3230 3520 3539   978393.96205 59
-00003480: 3438 3633 352e 3238 3930 3136 2929 721d  48635.289016))r.
-00003490: 0000 0072 4400 0000 7ac5 5352 4944 3d34  ...rD...z.SRID=4
-000034a0: 3332 363b 504f 4c59 474f 4e20 2828 382e  326;POLYGON ((8.
-000034b0: 3738 3930 3632 3439 3939 3937 3720 3437  7890624999977 47
-000034c0: 2e30 3430 3138 3231 3433 3237 3838 392c  .04018214327889,
-000034d0: 2031 342e 3036 3234 3939 3939 3939 3936   14.062499999996
-000034e0: 3332 2034 372e 3034 3031 3832 3134 3332  32 47.0401821432
-000034f0: 3738 3839 2c20 3134 2e30 3632 3439 3939  7889, 14.0624999
-00003500: 3939 3939 3633 3220 3530 2e37 3336 3435  9999632 50.73645
-00003510: 3531 3335 3539 3039 2c20 382e 3738 3930  51355909, 8.7890
-00003520: 3632 3439 3939 3937 3720 3530 2e37 3336  624999977 50.736
-00003530: 3435 3531 3335 3539 3039 2c20 382e 3738  4551355909, 8.78
-00003540: 3930 3632 3439 3939 3937 3720 3437 2e30  90624999977 47.0
-00003550: 3430 3138 3231 3433 3237 3838 3929 2929  4018214327889)))
-00003560: 0c72 0b00 0000 720e 0000 0072 2000 0000  .r....r....r ...
-00003570: 7209 0000 0072 8e00 0000 723d 0000 0072  r....r....r=...r
-00003580: 1200 0000 5a15 736e 6170 5f76 6965 7770  ....Z.snap_viewp
-00003590: 6f72 745f 746f 5f67 7269 6472 2100 0000  ort_to_gridr!...
-000035a0: da03 7374 7272 3700 0000 7248 0000 0029  ..strr7...rH...)
-000035b0: 0a72 2700 0000 722b 0000 0072 2c00 0000  .r'...r+...r,...
-000035c0: 7228 0000 0072 2900 0000 7222 0000 0072  r(...r)...r"...r
-000035d0: 2d00 0000 7239 0000 005a 0e67 7269 645f  -...r9...Z.grid_
-000035e0: 7265 6374 616e 676c 655a 0c70 6f6c 7967  rectangleZ.polyg
-000035f0: 6f6e 5f34 3332 3672 2e00 0000 722e 0000  on_4326r....r...
-00003600: 0072 2f00 0000 da1a 7465 7374 5f73 6e61  .r/.....test_sna
-00003610: 705f 7669 6577 706f 7274 5f74 6f5f 6772  p_viewport_to_gr
-00003620: 6964 b902 0000 731a 0000 0000 0204 0104  id....s.........
-00003630: 0208 0108 0210 020c 030a 020c 0210 010e  ................
-00003640: 020a 0204 027a 3854 6573 744d 6170 436c  .....z8TestMapCl
-00003650: 7573 7465 7265 7243 6f6e 7465 6e74 436f  ustererContentCo
-00003660: 756e 7473 2e74 6573 745f 736e 6170 5f76  unts.test_snap_v
-00003670: 6965 7770 6f72 745f 746f 5f67 7269 6463  iewport_to_gridc
-00003680: 0100 0000 0000 0000 0000 0000 0c00 0000  ................
-00003690: 0a00 0000 4300 0000 73bc 0000 0064 017d  ....C...s....d.}
-000036a0: 0167 007d 027c 00a0 0064 0264 03a1 0201  .g.}.|...d.d....
-000036b0: 007c 00a0 0064 0464 05a1 0201 0074 0144  .|...d.d.....t.D
-000036c0: 005d 927d 0374 0244 005d 887d 0474 0374  .].}.t.D.].}.t.t
-000036d0: 0474 0574 0666 0444 005d 767d 057c 00a0  .t.t.f.D.]v}.|..
-000036e0: 077c 047c 017c 037c 02a1 047d 0674 087c  .|.|.|.|...}.t.|
-000036f0: 0674 0964 068d 027d 0764 077d 087c 07a0  .t.d...}.d.}.|..
-00003700: 0a7c 057c 047c 017c 027c 08a1 057d 097c  .|.|.|.|.|...}.|
-00003710: 0474 0b6b 0272 9864 0864 0969 0164 0864  .t.k.r.d.d.i.d.d
-00003720: 0969 0164 0a9c 027d 0a7c 00a0 0c7c 097c  .i.d...}.|...|.|
-00003730: 0aa1 0201 0074 0d6a 0ea0 0fa1 007d 0b7c  .....t.j.....}.|
-00003740: 00a0 0c7c 0ba0 10a1 0064 0ba1 0201 0071  ...|.....d.....q
-00003750: 3c71 2c71 2464 0053 0029 0c4e 726a 0000  <q,q$d.S.).Nrj..
-00003760: 0072 8b00 0000 7282 0000 0072 8c00 0000  .r....r....r....
-00003770: 728d 0000 0072 8900 0000 7254 0000 0072  r....r....rT...r
-00003780: 6100 0000 7231 0000 0029 0272 8200 0000  a...r1...).r....
-00003790: 728d 0000 0072 3300 0000 2911 728f 0000  r....r3...).r...
-000037a0: 0072 0b00 0000 720e 0000 0072 1100 0000  .r....r....r....
-000037b0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-000037c0: 2000 0000 7209 0000 0072 8e00 0000 da18   ...r....r......
-000037d0: 6765 745f 6772 6f75 7065 645f 6d61 705f  get_grouped_map_
-000037e0: 636f 6e74 656e 7473 720c 0000 0072 2100  contentsr....r!.
-000037f0: 0000 7218 0000 0072 7200 0000 7273 0000  ..r....rr...rs..
-00003800: 0072 6100 0000 290c 7227 0000 0072 2c00  .ra...).r'...r,.
-00003810: 0000 722b 0000 0072 2800 0000 7229 0000  ..r+...r(...r)..
-00003820: 0072 3800 0000 7222 0000 0072 2d00 0000  .r8...r"...r-...
-00003830: da08 6772 6f75 705f 6279 7291 0000 0072  ..group_byr....r
-00003840: 9200 0000 7293 0000 0072 2e00 0000 722e  ....r....r....r.
-00003850: 0000 0072 2f00 0000 da1d 7465 7374 5f67  ...r/.....test_g
-00003860: 6574 5f67 726f 7570 6564 5f6d 6170 5f63  et_grouped_map_c
-00003870: 6f6e 7465 6e74 73d3 0200 0073 2c00 0000  ontents....s,...
-00003880: 0002 0401 0402 0c01 0c02 0801 0802 1002  ................
-00003890: 1002 0c02 0402 1202 0804 0200 02ff 0204  ................
-000038a0: 0200 02ff 02fc 0609 0c02 0a01 7a3b 5465  ............z;Te
-000038b0: 7374 4d61 7043 6c75 7374 6572 6572 436f  stMapClustererCo
-000038c0: 6e74 656e 7443 6f75 6e74 732e 7465 7374  ntentCounts.test
-000038d0: 5f67 6574 5f67 726f 7570 6564 5f6d 6170  _get_grouped_map
-000038e0: 5f63 6f6e 7465 6e74 734e 2908 727e 0000  _contentsN).r~..
-000038f0: 0072 7f00 0000 7280 0000 0072 9400 0000  .r....r....r....
-00003900: 7298 0000 0072 9b00 0000 729d 0000 0072  r....r....r....r
-00003910: a000 0000 722e 0000 0072 2e00 0000 722e  ....r....r....r.
-00003920: 0000 0072 2f00 0000 7281 0000 00e0 0100  ...r/...r.......
-00003930: 0073 0a00 0000 0802 0876 0844 081d 081a  .s.......v.D....
-00003940: 7281 0000 0072 5500 0000 7257 0000 0029  r....rU...rW...)
-00003950: 01da 2641 4e59 434c 5553 5445 525f 4144  ..&ANYCLUSTER_AD
-00003960: 4449 5449 4f4e 414c 5f47 524f 5550 5f42  DITIONAL_GROUP_B
-00003970: 595f 434f 4c55 4d4e 5363 0000 0000 0000  Y_COLUMNSc......
-00003980: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00003990: 0000 731c 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000039a0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
-000039b0: 0553 0029 06da 2354 6573 744d 6170 436c  .S.)..#TestMapCl
-000039c0: 7573 7465 7265 7241 6c74 6572 6e61 7469  ustererAlternati
-000039d0: 7665 5365 7474 696e 6773 6301 0000 0000  veSettingsc.....
-000039e0: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
-000039f0: 0000 0073 6600 0000 6401 7d01 6700 7d02  ...sf...d.}.g.}.
-00003a00: 7400 4400 5d54 7d03 7401 4400 5d4a 7d04  t.D.]T}.t.D.]J}.
-00003a10: 7402 7403 7404 7405 6604 4400 5d38 7d05  t.t.t.t.f.D.]8}.
-00003a20: 7c00 a006 7c04 7c01 7c03 7c02 a104 7d06  |...|.|.|.|...}.
-00003a30: 7407 7c06 7408 6402 8d02 7d07 7c07 a009  t.|.t.d...}.|...
-00003a40: a100 7d08 6403 7d09 7c00 a00a 7c08 7c09  ..}.d.}.|...|.|.
-00003a50: a102 0100 7124 7114 710c 6400 5300 2904  ....q$q.q.d.S.).
-00003a60: 4e72 6a00 0000 7289 0000 007a 4c2c 204d  Nrj...r....zL, M
-00003a70: 494e 2872 6174 696e 673a 3a56 4152 4348  IN(rating::VARCH
-00003a80: 4152 2920 4153 2072 6174 696e 672c 204d  AR) AS rating, M
-00003a90: 494e 286c 6173 745f 7265 6e65 7761 6c3a  IN(last_renewal:
-00003aa0: 3a56 4152 4348 4152 2920 4153 206c 6173  :VARCHAR) AS las
-00003ab0: 745f 7265 6e65 7761 6c29 0b72 0b00 0000  t_renewal).r....
-00003ac0: 720e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00003ad0: 1300 0000 7214 0000 0072 2000 0000 7209  ....r....r ...r.
-00003ae0: 0000 0072 8e00 0000 5a26 6765 745f 6164  ...r....Z&get_ad
-00003af0: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
-00003b00: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
-00003b10: 7221 0000 0029 0a72 2700 0000 722c 0000  r!...).r'...r,..
-00003b20: 0072 2b00 0000 7228 0000 0072 2900 0000  .r+...r(...r)...
-00003b30: 7238 0000 0072 2200 0000 722d 0000 005a  r8...r"...r-...Z
-00003b40: 0e63 6f6c 756d 6e73 5f73 7472 696e 6772  .columns_stringr
-00003b50: 6800 0000 722e 0000 0072 2e00 0000 722f  h...r....r....r/
-00003b60: 0000 00da 2b74 6573 745f 6765 745f 6164  ....+test_get_ad
-00003b70: 6469 7469 6f6e 616c 5f67 726f 7570 5f62  ditional_group_b
-00003b80: 795f 636f 6c75 6d6e 735f 7374 7269 6e67  y_columns_string
-00003b90: fd02 0000 7314 0000 0000 0204 0104 0208  ....s...........
-00003ba0: 0108 0210 0210 020c 0208 0204 017a 4f54  .............zOT
-00003bb0: 6573 744d 6170 436c 7573 7465 7265 7241  estMapClustererA
-00003bc0: 6c74 6572 6e61 7469 7665 5365 7474 696e  lternativeSettin
-00003bd0: 6773 2e74 6573 745f 6765 745f 6164 6469  gs.test_get_addi
-00003be0: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
-00003bf0: 636f 6c75 6d6e 735f 7374 7269 6e67 6301  columns_stringc.
-00003c00: 0000 0000 0000 0000 0000 000c 0000 000a  ................
-00003c10: 0000 0043 0000 0073 be00 0000 6401 7d01  ...C...s....d.}.
-00003c20: 6700 7d02 7c00 a000 6402 6403 a102 0100  g.}.|...d.d.....
-00003c30: 7c00 a000 6404 6405 a102 0100 7c00 a001  |...d.d.....|...
-00003c40: 7402 7403 6406 8302 a101 0100 7404 4400  t.t.d.......t.D.
-00003c50: 5d84 7d03 7405 4400 5d7a 7d04 7406 7407  ].}.t.D.]z}.t.t.
-00003c60: 7408 7409 6604 4400 5d68 7d05 7c00 a00a  t.t.f.D.]h}.|...
-00003c70: 7c04 7c01 7c03 7c02 a104 7d06 740b 7c06  |.|.|.|...}.t.|.
-00003c80: 740c 6407 8d02 7d07 6408 7d08 7c07 a00d  t.d...}.d.}.|...
-00003c90: 7c05 7c04 7c01 7c02 7c08 a105 7d09 7c04  |.|.|.|.|...}.|.
-00003ca0: 740e 6b02 724c 7c09 a00f a100 4400 5d20  t.k.rL|.....D.] 
-00003cb0: 5c02 7d0a 7d0b 7c00 a010 6409 7c0b a102  \.}.}.|...d.|...
-00003cc0: 0100 7c00 a010 640a 7c0b a102 0100 7192  ..|...d.|.....q.
-00003cd0: 714c 713c 7134 6400 5300 290b 4e72 6a00  qLq<q4d.S.).Nrj.
-00003ce0: 0000 728b 0000 0072 8200 0000 728c 0000  ..r....r....r...
-00003cf0: 0072 8d00 0000 72a1 0000 0072 8900 0000  .r....r....r....
-00003d00: 7254 0000 0072 5500 0000 7257 0000 0029  rT...rU...rW...)
-00003d10: 1172 8f00 0000 7235 0000 00da 0768 6173  .r....r5.....has
-00003d20: 6174 7472 7205 0000 0072 0b00 0000 720e  attrr....r....r.
-00003d30: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00003d40: 0000 7214 0000 0072 2000 0000 7209 0000  ..r....r ...r...
-00003d50: 0072 8e00 0000 729e 0000 0072 0c00 0000  .r....r....r....
-00003d60: da05 6974 656d 73da 0861 7373 6572 7449  ..items..assertI
-00003d70: 6e29 0c72 2700 0000 722c 0000 0072 2b00  n).r'...r,...r+.
-00003d80: 0000 7228 0000 0072 2900 0000 7238 0000  ..r(...r)...r8..
-00003d90: 0072 2200 0000 722d 0000 0072 9f00 0000  .r"...r-...r....
-00003da0: 7291 0000 00da 0961 6767 7265 6761 7465  r......aggregate
-00003db0: da04 6461 7461 722e 0000 0072 2e00 0000  ..datar....r....
-00003dc0: 722f 0000 00da 3074 6573 745f 6765 745f  r/....0test_get_
-00003dd0: 6772 6f75 7065 645f 6d61 705f 636f 6e74  grouped_map_cont
-00003de0: 656e 7473 5f61 6464 6974 696f 6e61 6c5f  ents_additional_
-00003df0: 636f 6c75 6d6e 7311 0300 0073 2000 0000  columns....s ...
-00003e00: 0002 0401 0402 0c01 0c02 1002 0801 0802  ................
-00003e10: 1002 1002 0c02 0402 1202 0802 1002 0c01  ................
-00003e20: 7a54 5465 7374 4d61 7043 6c75 7374 6572  zTTestMapCluster
-00003e30: 6572 416c 7465 726e 6174 6976 6553 6574  erAlternativeSet
-00003e40: 7469 6e67 732e 7465 7374 5f67 6574 5f67  tings.test_get_g
-00003e50: 726f 7570 6564 5f6d 6170 5f63 6f6e 7465  rouped_map_conte
-00003e60: 6e74 735f 6164 6469 7469 6f6e 616c 5f63  nts_additional_c
-00003e70: 6f6c 756d 6e73 4e29 0572 7e00 0000 727f  olumnsN).r~...r.
-00003e80: 0000 0072 8000 0000 72a3 0000 0072 a900  ...r....r....r..
-00003e90: 0000 722e 0000 0072 2e00 0000 722e 0000  ..r....r....r...
-00003ea0: 0072 2f00 0000 72a2 0000 00f9 0200 0073  .r/...r........s
-00003eb0: 0400 0000 0804 0814 72a2 0000 0029 27da  ........r....)'.
-00003ec0: 0b64 6a61 6e67 6f2e 7465 7374 7202 0000  .django.testr...
-00003ed0: 0072 0300 0000 7204 0000 00da 0b64 6a61  .r....r......dja
-00003ee0: 6e67 6f2e 636f 6e66 7205 0000 00da 1764  ngo.confr......d
-00003ef0: 6a61 6e67 6f2e 636f 6e74 7269 622e 6769  jango.contrib.gi
-00003f00: 732e 6765 6f73 7206 0000 00da 1764 6a61  s.geosr......dja
-00003f10: 6e67 6f2e 636f 6e74 7269 622e 6769 732e  ngo.contrib.gis.
-00003f20: 6764 616c 7207 0000 0072 0800 0000 5a17  gdalr....r....Z.
-00003f30: 616e 7963 6c75 7374 6572 2e4d 6170 436c  anycluster.MapCl
-00003f40: 7573 7465 7265 7272 0900 0000 da0a 616e  ustererr......an
-00003f50: 7963 6c75 7374 6572 720a 0000 00da 1661  yclusterr......a
-00003f60: 6e79 636c 7573 7465 722e 6465 6669 6e69  nycluster.defini
-00003f70: 7469 6f6e 7372 0b00 0000 720c 0000 0072  tionsr....r....r
-00003f80: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00003f90: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
-00003fa0: 7465 7374 732e 636f 6d6d 6f6e 7211 0000  tests.commonr...
-00003fb0: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00003fc0: 5a17 616e 7963 6c75 7374 6572 2e74 6573  Z.anycluster.tes
-00003fd0: 7473 2e6d 6978 696e 7372 1500 0000 7216  ts.mixinsr....r.
-00003fe0: 0000 0072 1700 0000 5a0d 616e 796d 6170  ...r....Z.anymap
-00003ff0: 2e6d 6f64 656c 7372 1800 0000 7246 0000  .modelsr....rF..
-00004000: 0072 1f00 0000 728e 0000 0072 1b00 0000  .r....r....r....
-00004010: 7281 0000 0072 a200 0000 722e 0000 0072  r....r....r....r
-00004020: 2e00 0000 722e 0000 0072 2f00 0000 da08  ....r....r/.....
-00004030: 3c6d 6f64 756c 653e 0100 0000 732a 0000  <module>....s*..
-00004040: 0014 010c 010c 0110 010c 010c 0220 0218  ............. ..
-00004050: 0114 020c 0208 0204 0104 0214 7f00 7f00  ................
-00004060: 7f00 4f14 7f00 7f00 1b0c 01              ..O........
+00002920: 005a 0764 0b64 0c84 005a 0864 0d53 0029  .Z.d.d...Z.d.S.)
+00002930: 0eda 1d54 6573 744d 6170 436c 7573 7465  ...TestMapCluste
+00002940: 7265 7243 6f6e 7465 6e74 436f 756e 7473  rerContentCounts
+00002950: 6301 0000 0000 0000 0000 0000 000f 0000  c...............
+00002960: 000a 0000 0043 0000 0073 cc01 0000 6401  .....C...s....d.
+00002970: 7d01 6402 6403 6404 6405 9c03 6701 7d02  }.d.d.d.d...g.}.
+00002980: 6406 6407 6408 6404 6405 9c03 6701 6901  d.d.d.d.d...g.i.
+00002990: 6406 6407 6408 6409 6405 9c03 6701 6901  d.d.d.d.d...g.i.
+000029a0: 640a 9c02 7d03 6407 6408 6404 6405 9c03  d...}.d.d.d.d...
+000029b0: 6407 6408 6409 6405 9c03 640a 9c02 7d04  d.d.d.d...d...}.
+000029c0: 7400 4400 9001 5d6e 7d05 7401 4400 9001  t.D...]n}.t.D...
+000029d0: 5d62 7d06 7402 7403 7404 7405 6604 4400  ]b}.t.t.t.t.f.D.
+000029e0: 9001 5d4e 7d07 7c05 7406 6b02 728a 7c06  ..]N}.|.t.k.r.|.
+000029f0: 7407 6b03 728a 7172 7c06 7407 6b02 729c  t.k.r.qr|.t.k.r.
+00002a00: 7c07 7403 6b03 729c 7172 7c00 a008 7c06  |.t.k.r.qr|...|.
+00002a10: 7c01 7c05 7c02 a104 7d08 7409 7c08 740a  |.|.|...}.t.|.t.
+00002a20: 640b 8d02 7d09 7c09 a00b 7c07 7c06 7c02  d...}.|...|.|.|.
+00002a30: 7c01 7c03 a105 7d0a 7c09 a00b 7c07 7c06  |.|...}.|...|.|.
+00002a40: 7c02 7c01 7c04 a105 0400 7d0b 7d0a 640c  |.|.|.....}.}.d.
+00002a50: 640d 640c 6901 640d 640c 6901 640a 9c02  d.d.i.d.d.i.d...
+00002a60: 640e 9c02 7d0c 7c00 a00c 7c0a 7c0c a102  d...}.|...|.|...
+00002a70: 0100 7c00 a00c 7c0b 7c0c a102 0100 7c06  ..|...|.|.....|.
+00002a80: 7407 6b02 9001 728a 7c00 a00d 640f 6403  t.k...r.|...d.d.
+00002a90: a102 0100 7c00 a00d 6410 6411 a102 0100  ....|...d.d.....
+00002aa0: 7c09 a00b 7c07 7c06 7c02 7c01 7c03 a105  |...|.|.|.|.|...
+00002ab0: 7d0a 7c09 a00b 7c07 7c06 7c02 7c01 7c04  }.|...|.|.|.|.|.
+00002ac0: a105 0400 7d0b 7d0a 6412 640d 640c 6901  ....}.}.d.d.d.i.
+00002ad0: 640d 6412 6901 640a 9c02 640e 9c02 7d0c  d.d.i.d...d...}.
+00002ae0: 7c00 a00c 7c0a 7c0c a102 0100 7c00 a00c  |...|.|.....|...
+00002af0: 7c0b 7c0c a102 0100 740e 6a0f a010 a100  |.|.....t.j.....
+00002b00: 7d0d 7c0d 4400 5d0e 7d0e 7c0e a011 a100  }.|.D.].}.|.....
+00002b10: 0100 9001 7198 740e 6a0f a010 a100 7d0d  ....q.t.j.....}.
+00002b20: 7c00 a00c 7c0d a012 a100 640c a102 0100  |...|.....d.....
+00002b30: 7172 7160 7156 6400 5300 2913 4e72 6a00  qrq`qVd.S.).Nrj.
+00002b40: 0000 7254 0000 00da 0573 746f 6e65 fa01  ..rT.....stone..
+00002b50: 3da9 03da 0663 6f6c 756d 6eda 0576 616c  =....column..val
+00002b60: 7565 da08 6f70 6572 6174 6f72 722b 0000  ue..operatorr+..
+00002b70: 0072 5600 0000 547a 0221 3d29 02da 0466  .rV...Tz.!=)...f
+00002b80: 7265 655a 0470 6169 64a9 0172 2500 0000  reeZ.paid..r%...
+00002b90: 7201 0000 0072 6100 0000 2902 7261 0000  r....ra...).ra..
+00002ba0: 00da 0b6d 6f64 756c 6174 696f 6e73 fa06  ...modulations..
+00002bb0: 6e61 6d65 2031 fa06 6e61 6d65 2032 da06  name 1..name 2..
+00002bc0: 666c 6f77 6572 7231 0000 0029 1372 0b00  flowerr1...).r..
+00002bd0: 0000 720e 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00002be0: 0072 1300 0000 7214 0000 0072 1000 0000  .r....r....r....
+00002bf0: 720c 0000 0072 2000 0000 7209 0000 00da  r....r ...r.....
+00002c00: 0e54 4553 545f 4752 4944 5f53 495a 455a  .TEST_GRID_SIZEZ
+00002c10: 1667 6574 5f6d 6170 5f63 6f6e 7465 6e74  .get_map_content
+00002c20: 5f63 6f75 6e74 7372 2100 0000 da0c 6372  _countsr!.....cr
+00002c30: 6561 7465 5f70 6f69 6e74 7218 0000 0072  eate_pointr....r
+00002c40: 7200 0000 7273 0000 00da 0664 656c 6574  r...rs.....delet
+00002c50: 6572 6100 0000 290f 7227 0000 0072 2c00  era...).r'...r,.
+00002c60: 0000 722b 0000 0072 8a00 0000 5a12 7369  ..r+...r....Z.si
+00002c70: 6d70 6c65 5f6d 6f64 756c 6174 696f 6e73  mple_modulations
+00002c80: 7228 0000 0072 2900 0000 7238 0000 0072  r(...r)...r8...r
+00002c90: 2200 0000 722d 0000 00da 0672 6573 756c  "...r-.....resul
+00002ca0: 745a 1e72 6573 756c 745f 6672 6f6d 5f73  tZ.result_from_s
+00002cb0: 696d 706c 655f 6d6f 6475 6c61 7469 6f6e  imple_modulation
+00002cc0: 73da 0f65 7870 6563 7465 645f 7265 7375  s..expected_resu
+00002cd0: 6c74 da07 6761 7264 656e 7372 7600 0000  lt..gardensrv...
+00002ce0: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
+00002cf0: 1b74 6573 745f 6765 745f 6d61 705f 636f  .test_get_map_co
+00002d00: 6e74 656e 745f 636f 756e 7473 e201 0000  ntent_counts....
+00002d10: 73a6 0000 0000 0204 0502 0102 0102 fd04  s...............
+00002d20: ff04 0b02 0202 0102 0102 fd04 ff02 fe02  ................
+00002d30: 0b02 0202 0102 0102 fd04 ff02 ff02 f506  ................
+00002d40: 1802 0102 0102 fd04 0602 0102 0102 fd04  ................
+00002d50: fa06 0e0a 010a 0212 0210 0102 0210 0102  ................
+00002d60: 0210 010c 0212 0206 0102 0002 0002 0002  ................
+00002d70: ff08 0402 0302 0002 ff02 0402 0002 ff02  ................
+00002d80: fc04 fe06 0b0c 010c 020a 020c 010c 0212  ................
+00002d90: 0106 0102 0002 0002 0002 ff08 0402 0302  ................
+00002da0: 0002 ff02 0402 0002 ff02 fc04 fe06 0e0c  ................
+00002db0: 010c 020a 0108 010c 030a 027a 3954 6573  ...........z9Tes
+00002dc0: 744d 6170 436c 7573 7465 7265 7243 6f6e  tMapClustererCon
+00002dd0: 7465 6e74 436f 756e 7473 2e74 6573 745f  tentCounts.test_
+00002de0: 6765 745f 6d61 705f 636f 6e74 656e 745f  get_map_content_
+00002df0: 636f 756e 7473 6301 0000 0000 0000 0000  countsc.........
+00002e00: 0000 000d 0000 0006 0000 0043 0000 0073  ...........C...s
+00002e10: 4001 0000 6401 7d01 7400 7d02 7401 7d03  @...d.}.t.}.t.}.
+00002e20: 6700 7d04 6700 7d05 7c00 a002 7c02 7c01  g.}.g.}.|...|.|.
+00002e30: 7c03 7c04 a104 7d06 7403 7c06 7404 6402  |.|...}.t.|.t.d.
+00002e40: 8d02 7d07 7405 7d08 7c07 a006 7c08 7c02  ..}.t.}.|...|.|.
+00002e50: 7c01 a103 7d09 7c07 a007 7c09 7c04 7c05  |...}.|...|.|.|.
+00002e60: a103 7d0a 7c00 a008 7c0a 6403 a102 0100  ..}.|...|.d.....
+00002e70: 7c00 a009 6404 6405 a102 0100 7c07 a007  |...d.d.....|...
+00002e80: 7c09 7c04 7c05 a103 7d0a 7c00 a008 7c0a  |.|.|...}.|...|.
+00002e90: 6406 a102 0100 7c00 a009 6407 6408 a102  d.....|...d.d...
+00002ea0: 0100 7c07 a007 7c09 7c04 7c05 a103 7d0a  ..|...|.|.|...}.
+00002eb0: 7c00 a008 7c0a 6409 a102 0100 640a 6405  |...|.d.....d.d.
+00002ec0: 640b 640c 9c03 6701 7d04 7c07 a007 7c09  d.d...g.}.|...|.
+00002ed0: 7c04 7c05 a103 7d0a 7c00 a008 7c0a 6406  |.|...}.|...|.d.
+00002ee0: a102 0100 640a 6405 640b 640c 9c03 640a  ....d.d.d.d...d.
+00002ef0: 6408 640b 640d 640e 9c04 6702 7d04 7c07  d.d.d.d...g.}.|.
+00002f00: a007 7c09 7c04 7c05 a103 7d0a 7c00 a008  ..|.|.|...}.|...
+00002f10: 7c0a 6409 a102 0100 740a 6a0b a00c a100  |.d.....t.j.....
+00002f20: 7d0b 7c0b 4400 5d0e 7d0c 7c0c a00d a100  }.|.D.].}.|.....
+00002f30: 0100 9001 7112 740a 6a0b a00c a100 7d0b  ....q.t.j.....}.
+00002f40: 7c00 a008 7c0b a00e a100 6403 a102 0100  |...|.....d.....
+00002f50: 6400 5300 290f 4e72 6a00 0000 7289 0000  d.S.).Nrj...r...
+00002f60: 0072 0100 0000 728b 0000 0072 8200 0000  .r....r....r....
+00002f70: 7231 0000 0072 8c00 0000 728d 0000 0072  r1...r....r....r
+00002f80: 3300 0000 7254 0000 0072 8300 0000 7284  3...rT...r....r.
+00002f90: 0000 00da 024f 52a9 0472 8500 0000 7286  .....OR..r....r.
+00002fa0: 0000 0072 8700 0000 da0f 6c6f 6769 6361  ...r......logica
+00002fb0: 6c4f 7065 7261 746f 7229 0f72 0c00 0000  lOperator).r....
+00002fc0: 720f 0000 0072 2000 0000 7209 0000 0072  r....r ...r....r
+00002fd0: 8e00 0000 7212 0000 00da 1b67 6574 5f67  ....r......get_g
+00002fe0: 656f 6d65 7472 6965 735f 666f 725f 636f  eometries_for_co
+00002ff0: 756e 7469 6e67 da17 7175 6572 795f 6d61  unting..query_ma
+00003000: 705f 636f 6e74 656e 745f 636f 756e 7472  p_content_countr
+00003010: 2100 0000 728f 0000 0072 1800 0000 7272  !...r....r....rr
+00003020: 0000 0072 7300 0000 7290 0000 0072 6100  ...rs...r....ra.
+00003030: 0000 290d 7227 0000 0072 2c00 0000 7229  ..).r'...r,...r)
+00003040: 0000 0072 2800 0000 722b 0000 005a 126d  ...r(...r+...Z.m
+00003050: 6f64 756c 6174 696f 6e5f 6669 6c74 6572  odulation_filter
+00003060: 7372 2200 0000 722d 0000 0072 3800 0000  sr"...r-...r8...
+00003070: da17 6765 6f6d 6574 7269 6573 5f66 6f72  ..geometries_for
+00003080: 5f63 6f75 6e74 696e 6772 6100 0000 7293  _countingra...r.
+00003090: 0000 0072 7600 0000 722e 0000 0072 2e00  ...rv...r....r..
+000030a0: 0000 722f 0000 00da 1c74 6573 745f 7175  ..r/.....test_qu
+000030b0: 6572 795f 6d61 705f 636f 6e74 656e 745f  ery_map_content_
+000030c0: 636f 756e 7458 0200 0073 5200 0000 0002  countX...sR.....
+000030d0: 0401 0401 0403 0401 0402 1001 0c02 0402  ................
+000030e0: 0e02 0e01 0c02 0c02 0e01 0c02 0c02 0e01  ................
+000030f0: 0c05 0201 0201 02fd 04ff 0408 0e01 0c04  ................
+00003100: 0201 0201 02fd 0406 0201 0201 0201 02fc  ................
+00003110: 04fa 040e 0e01 0c02 0a01 0801 0c02 0a02  ................
+00003120: 7a3a 5465 7374 4d61 7043 6c75 7374 6572  z:TestMapCluster
+00003130: 6572 436f 6e74 656e 7443 6f75 6e74 732e  erContentCounts.
+00003140: 7465 7374 5f71 7565 7279 5f6d 6170 5f63  test_query_map_c
+00003150: 6f6e 7465 6e74 5f63 6f75 6e74 6301 0000  ontent_countc...
+00003160: 0000 0000 0000 0000 0012 0000 0006 0000  ................
+00003170: 0043 0000 0073 1801 0000 6401 7d01 7400  .C...s....d.}.t.
+00003180: 7d02 7401 7d03 6402 6403 6404 6405 9c03  }.t.}.d.d.d.d...
+00003190: 6402 6406 6404 6407 6408 9c04 6702 7d04  d.d.d.d.d...g.}.
+000031a0: 7c00 a002 7c02 7c01 7c03 7c04 a104 7d05  |...|.|.|.|...}.
+000031b0: 7403 7c05 7404 6409 8d02 7d06 7405 7d07  t.|.t.d...}.t.}.
+000031c0: 7c06 a006 7c07 7c02 7c01 a103 7d08 6402  |...|.|.|...}.d.
+000031d0: 6403 6404 6405 9c03 6701 7d09 7c00 a007  d.d.d...g.}.|...
+000031e0: 640a 6403 a102 7d0a 7c00 a007 640b 6406  d.d...}.|...d.d.
+000031f0: a102 7d0b 7c00 a007 640c 6403 a102 7d0c  ..}.|...d.d...}.
+00003200: 7c00 a007 640d 6403 a102 7d0d 7c00 a007  |...d.d...}.|...
+00003210: 640e 6403 a102 7d0e 7c00 a007 640f 6403  d.d...}.|...d.d.
+00003220: a102 7d0f 6410 7c0a 5f08 7c0a a009 a100  ..}.d.|._.|.....
+00003230: 0100 6410 7c0c 5f08 7c0c a009 a100 0100  ..d.|._.|.......
+00003240: 7c06 a00a 7c08 7c04 7c09 a103 7d10 7c00  |...|.|.|...}.|.
+00003250: a00b 7c10 6411 a102 0100 6402 6403 6404  ..|.d.....d.d.d.
+00003260: 6405 9c03 6412 6410 6404 6413 6408 9c04  d...d.d.d.d.d...
+00003270: 6702 7d11 7c06 a00a 7c08 7c04 7c11 a103  g.}.|...|.|.|...
+00003280: 7d10 7c00 a00b 7c10 6414 a102 0100 6400  }.|...|.d.....d.
+00003290: 5300 2915 4e72 6a00 0000 7254 0000 0072  S.).Nrj...rT...r
+000032a0: 8200 0000 7283 0000 0072 8400 0000 728d  ....r....r....r.
+000032b0: 0000 0072 9500 0000 7296 0000 0072 8900  ...r....r....r..
+000032c0: 0000 728b 0000 0072 8c00 0000 7a06 6e61  ..r....r....z.na
+000032d0: 6d65 2033 7a06 6e61 6d65 2034 7a06 6e61  me 3z.name 4z.na
+000032e0: 6d65 2035 7a06 6e61 6d65 2036 54e9 0500  me 5z.name 6T...
+000032f0: 0000 7256 0000 00da 0341 4e44 7233 0000  ..rV.....ANDr3..
+00003300: 0029 0c72 0c00 0000 720f 0000 0072 2000  .).r....r....r .
+00003310: 0000 7209 0000 0072 8e00 0000 7212 0000  ..r....r....r...
+00003320: 0072 9800 0000 728f 0000 0072 5600 0000  .r....r....rV...
+00003330: da04 7361 7665 7299 0000 0072 2100 0000  ..saver....r!...
+00003340: 2912 7227 0000 0072 2c00 0000 7229 0000  ).r'...r,...r)..
+00003350: 0072 2800 0000 722b 0000 0072 2200 0000  .r(...r+...r"...
+00003360: 722d 0000 0072 3800 0000 729a 0000 005a  r-...r8...r....Z
+00003370: 1073 746f 6e65 5f6d 6f64 756c 6174 696f  .stone_modulatio
+00003380: 6e5a 0867 6172 6465 6e5f 315a 0867 6172  nZ.garden_1Z.gar
+00003390: 6465 6e5f 325a 0867 6172 6465 6e5f 335a  den_2Z.garden_3Z
+000033a0: 0867 6172 6465 6e5f 345a 0867 6172 6465  .garden_4Z.garde
+000033b0: 6e5f 355a 0867 6172 6465 6e5f 3672 6100  n_5Z.garden_6ra.
+000033c0: 0000 5a15 7374 6f6e 655f 6672 6565 5f6d  ..Z.stone_free_m
+000033d0: 6f64 756c 6174 696f 6e72 2e00 0000 722e  odulationr....r.
+000033e0: 0000 0072 2f00 0000 da2d 7465 7374 5f71  ...r/....-test_q
+000033f0: 7565 7279 5f6d 6170 5f63 6f6e 7465 6e74  uery_map_content
+00003400: 5f63 6f75 6e74 5f77 6974 685f 6d6f 6475  _count_with_modu
+00003410: 6c61 7469 6f6e 739c 0200 0073 5a00 0000  lations....sZ...
+00003420: 0002 0401 0401 0404 0201 0201 02fd 0406  ................
+00003430: 0201 0201 0201 02fc 04fa 040e 1001 0c02  ................
+00003440: 0402 0e04 0201 0201 02fd 0807 0c01 0c01  ................
+00003450: 0c01 0c01 0c01 0c02 0601 0801 0601 0802  ................
+00003460: 0e01 0c04 0201 0201 02fd 0406 0201 0201  ................
+00003470: 0201 02fc 04fa 040e 0e01 7a4b 5465 7374  ..........zKTest
+00003480: 4d61 7043 6c75 7374 6572 6572 436f 6e74  MapClustererCont
+00003490: 656e 7443 6f75 6e74 732e 7465 7374 5f71  entCounts.test_q
+000034a0: 7565 7279 5f6d 6170 5f63 6f6e 7465 6e74  uery_map_content
+000034b0: 5f63 6f75 6e74 5f77 6974 685f 6d6f 6475  _count_with_modu
+000034c0: 6c61 7469 6f6e 7363 0100 0000 0000 0000  lationsc........
+000034d0: 0000 0000 0a00 0000 0900 0000 4300 0000  ............C...
+000034e0: 73aa 0000 0064 017d 0174 0044 005d 9c7d  s....d.}.t.D.].}
+000034f0: 0274 0144 005d 927d 0374 0274 0374 0474  .t.D.].}.t.t.t.t
+00003500: 0566 0444 005d 807d 047c 0274 066b 0272  .f.D.].}.|.t.k.r
+00003510: 367c 0374 076b 0372 3671 207c 0374 076b  6|.t.k.r6q |.t.k
+00003520: 0272 487c 0474 036b 0372 4871 2067 007d  .rH|.t.k.rHq g.}
+00003530: 057c 00a0 087c 037c 017c 027c 05a1 047d  .|...|.|.|.|...}
+00003540: 0674 097c 0674 0a64 028d 027d 077c 07a0  .t.|.t.d...}.|..
+00003550: 0b7c 047c 037c 01a1 037d 087c 00a0 0c74  .|.|.|...}.|...t
+00003560: 0d7c 0874 0e83 02a1 0101 007c 0844 005d  .|.t.......|.D.]
+00003570: 147d 097c 00a0 0c64 037c 096a 0f6b 06a1  .}.|...d.|.j.k..
+00003580: 0101 0071 8a71 2071 1071 0864 0053 0029  ...q.q q.q.d.S.)
+00003590: 044e 726a 0000 0072 8900 0000 da07 504f  .Nrj...r......PO
+000035a0: 4c59 474f 4e29 1072 0b00 0000 720e 0000  LYGON).r....r...
+000035b0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000035c0: 7214 0000 0072 1000 0000 720c 0000 0072  r....r....r....r
+000035d0: 2000 0000 7209 0000 0072 8e00 0000 7298   ...r....r....r.
+000035e0: 0000 0072 3500 0000 7236 0000 0072 6300  ...r5...r6...rc.
+000035f0: 0000 da03 776b 7429 0a72 2700 0000 722c  ....wkt).r'...r,
+00003600: 0000 0072 2800 0000 7229 0000 0072 3800  ...r(...r)...r8.
+00003610: 0000 722b 0000 0072 2200 0000 722d 0000  ..r+...r"...r-..
+00003620: 0072 3900 0000 7243 0000 0072 2e00 0000  .r9...rC...r....
+00003630: 722e 0000 0072 2f00 0000 da20 7465 7374  r....r/.... test
+00003640: 5f67 6574 5f67 656f 6d65 7472 6965 735f  _get_geometries_
+00003650: 666f 725f 636f 756e 7469 6e67 df02 0000  for_counting....
+00003660: 731e 0000 0000 0204 0208 0108 0210 0210  s...............
+00003670: 0102 0210 0102 0204 0210 010c 020e 0210  ................
+00003680: 0208 027a 3e54 6573 744d 6170 436c 7573  ...z>TestMapClus
+00003690: 7465 7265 7243 6f6e 7465 6e74 436f 756e  tererContentCoun
+000036a0: 7473 2e74 6573 745f 6765 745f 6765 6f6d  ts.test_get_geom
+000036b0: 6574 7269 6573 5f66 6f72 5f63 6f75 6e74  etries_for_count
+000036c0: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
+000036d0: 0a00 0000 0800 0000 4300 0000 738e 0000  ........C...s...
+000036e0: 0067 007d 0164 017d 0274 0044 005d 7c7d  .g.}.d.}.t.D.]|}
+000036f0: 0374 0144 005d 727d 047c 00a0 027c 047c  .t.D.]r}.|...|.|
+00003700: 027c 037c 01a1 047d 0574 037c 0574 0464  .|.|...}.t.|.t.d
+00003710: 028d 027d 067c 06a0 0574 06a1 017d 077c  ...}.|...t...}.|
+00003720: 06a0 077c 077c 02a1 027d 087c 00a0 0874  ...|.|...}.|...t
+00003730: 097c 0883 0164 03a1 0201 007c 00a0 087c  .|...d.....|...|
+00003740: 086a 0a64 04a1 0201 007c 08a0 0b64 05a1  .j.d.....|...d..
+00003750: 0101 0064 067d 097c 00a0 087c 0974 097c  ...d.}.|...|.t.|
+00003760: 0883 01a1 0201 0071 1471 0c64 0053 0029  .......q.q.d.S.)
+00003770: 074e 726a 0000 0072 8900 0000 7aa7 5352  .Nrj...r....z.SR
+00003780: 4944 3d33 3835 373b 504f 4c59 474f 4e20  ID=3857;POLYGON 
+00003790: 2828 3937 3833 3933 2e39 3632 3035 2035  ((978393.96205 5
+000037a0: 3934 3836 3335 2e32 3839 3031 362c 2031  948635.289016, 1
+000037b0: 3536 3534 3330 2e33 3339 3238 2035 3934  565430.33928 594
+000037c0: 3836 3335 2e32 3839 3031 362c 2031 3536  8635.289016, 156
+000037d0: 3534 3330 2e33 3339 3238 2036 3537 3438  5430.33928 65748
+000037e0: 3037 2e34 3234 3732 382c 2039 3738 3339  07.424728, 97839
+000037f0: 332e 3936 3230 3520 3635 3734 3830 372e  3.96205 6574807.
+00003800: 3432 3437 3238 2c20 3937 3833 3933 2e39  424728, 978393.9
+00003810: 3632 3035 2035 3934 3836 3335 2e32 3839  6205 5948635.289
+00003820: 3031 3629 2972 1d00 0000 7244 0000 007a  016))r....rD...z
+00003830: c553 5249 443d 3433 3236 3b50 4f4c 5947  .SRID=4326;POLYG
+00003840: 4f4e 2028 2838 2e37 3839 3036 3234 3939  ON ((8.789062499
+00003850: 3939 3737 2034 372e 3034 3031 3832 3134  9977 47.04018214
+00003860: 3332 3738 3839 2c20 3134 2e30 3632 3439  327889, 14.06249
+00003870: 3939 3939 3939 3633 3220 3437 2e30 3430  999999632 47.040
+00003880: 3138 3231 3433 3237 3838 392c 2031 342e  18214327889, 14.
+00003890: 3036 3234 3939 3939 3939 3936 3332 2035  06249999999632 5
+000038a0: 302e 3733 3634 3535 3133 3535 3930 392c  0.7364551355909,
+000038b0: 2038 2e37 3839 3036 3234 3939 3939 3737   8.7890624999977
+000038c0: 2035 302e 3733 3634 3535 3133 3535 3930   50.736455135590
+000038d0: 392c 2038 2e37 3839 3036 3234 3939 3939  9, 8.78906249999
+000038e0: 3737 2034 372e 3034 3031 3832 3134 3332  77 47.0401821432
+000038f0: 3738 3839 2929 290c 720b 0000 0072 0e00  7889))).r....r..
+00003900: 0000 7220 0000 0072 0900 0000 728e 0000  ..r ...r....r...
+00003910: 0072 3d00 0000 7212 0000 005a 1573 6e61  .r=...r....Z.sna
+00003920: 705f 7669 6577 706f 7274 5f74 6f5f 6772  p_viewport_to_gr
+00003930: 6964 7221 0000 00da 0373 7472 7237 0000  idr!.....strr7..
+00003940: 0072 4800 0000 290a 7227 0000 0072 2b00  .rH...).r'...r+.
+00003950: 0000 722c 0000 0072 2800 0000 7229 0000  ..r,...r(...r)..
+00003960: 0072 2200 0000 722d 0000 0072 3900 0000  .r"...r-...r9...
+00003970: 5a0e 6772 6964 5f72 6563 7461 6e67 6c65  Z.grid_rectangle
+00003980: 5a0c 706f 6c79 676f 6e5f 3433 3236 722e  Z.polygon_4326r.
+00003990: 0000 0072 2e00 0000 722f 0000 00da 1a74  ...r....r/.....t
+000039a0: 6573 745f 736e 6170 5f76 6965 7770 6f72  est_snap_viewpor
+000039b0: 745f 746f 5f67 7269 64fc 0200 0073 1a00  t_to_grid....s..
+000039c0: 0000 0002 0401 0402 0801 0802 1002 0c03  ................
+000039d0: 0a02 0c02 1001 0e02 0a02 0402 7a38 5465  ............z8Te
+000039e0: 7374 4d61 7043 6c75 7374 6572 6572 436f  stMapClustererCo
+000039f0: 6e74 656e 7443 6f75 6e74 732e 7465 7374  ntentCounts.test
+00003a00: 5f73 6e61 705f 7669 6577 706f 7274 5f74  _snap_viewport_t
+00003a10: 6f5f 6772 6964 6301 0000 0000 0000 0000  o_gridc.........
+00003a20: 0000 000c 0000 000a 0000 0043 0000 0073  ...........C...s
+00003a30: bc00 0000 6401 7d01 6700 7d02 7c00 a000  ....d.}.g.}.|...
+00003a40: 6402 6403 a102 0100 7c00 a000 6404 6405  d.d.....|...d.d.
+00003a50: a102 0100 7401 4400 5d92 7d03 7402 4400  ....t.D.].}.t.D.
+00003a60: 5d88 7d04 7403 7404 7405 7406 6604 4400  ].}.t.t.t.t.f.D.
+00003a70: 5d76 7d05 7c00 a007 7c04 7c01 7c03 7c02  ]v}.|...|.|.|.|.
+00003a80: a104 7d06 7408 7c06 7409 6406 8d02 7d07  ..}.t.|.t.d...}.
+00003a90: 6407 7d08 7c07 a00a 7c05 7c04 7c01 7c02  d.}.|...|.|.|.|.
+00003aa0: 7c08 a105 7d09 7c04 740b 6b02 7298 6408  |...}.|.t.k.r.d.
+00003ab0: 6409 6901 6408 6409 6901 640a 9c02 7d0a  d.i.d.d.i.d...}.
+00003ac0: 7c00 a00c 7c09 7c0a a102 0100 740d 6a0e  |...|.|.....t.j.
+00003ad0: a00f a100 7d0b 7c00 a00c 7c0b a010 a100  ....}.|...|.....
+00003ae0: 640b a102 0100 713c 712c 7124 6400 5300  d.....q<q,q$d.S.
+00003af0: 290c 4e72 6a00 0000 728b 0000 0072 8200  ).Nrj...r....r..
+00003b00: 0000 728c 0000 0072 8d00 0000 7289 0000  ..r....r....r...
+00003b10: 0072 5400 0000 7261 0000 0072 3100 0000  .rT...ra...r1...
+00003b20: 2902 7282 0000 0072 8d00 0000 7233 0000  ).r....r....r3..
+00003b30: 0029 1172 8f00 0000 720b 0000 0072 0e00  .).r....r....r..
+00003b40: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00003b50: 0072 1400 0000 7220 0000 0072 0900 0000  .r....r ...r....
+00003b60: 728e 0000 00da 1867 6574 5f67 726f 7570  r......get_group
+00003b70: 6564 5f6d 6170 5f63 6f6e 7465 6e74 7372  ed_map_contentsr
+00003b80: 0c00 0000 7221 0000 0072 1800 0000 7272  ....r!...r....rr
+00003b90: 0000 0072 7300 0000 7261 0000 0029 0c72  ...rs...ra...).r
+00003ba0: 2700 0000 722c 0000 0072 2b00 0000 7228  '...r,...r+...r(
+00003bb0: 0000 0072 2900 0000 7238 0000 0072 2200  ...r)...r8...r".
+00003bc0: 0000 722d 0000 00da 0867 726f 7570 5f62  ..r-.....group_b
+00003bd0: 7972 9100 0000 7292 0000 0072 9300 0000  yr....r....r....
+00003be0: 722e 0000 0072 2e00 0000 722f 0000 00da  r....r....r/....
+00003bf0: 1d74 6573 745f 6765 745f 6772 6f75 7065  .test_get_groupe
+00003c00: 645f 6d61 705f 636f 6e74 656e 7473 1603  d_map_contents..
+00003c10: 0000 732c 0000 0000 0204 0104 020c 010c  ..s,............
+00003c20: 0208 0108 0210 0210 020c 0204 0212 0208  ................
+00003c30: 0402 0002 ff02 0402 0002 ff02 fc06 090c  ................
+00003c40: 020a 017a 3b54 6573 744d 6170 436c 7573  ...z;TestMapClus
+00003c50: 7465 7265 7243 6f6e 7465 6e74 436f 756e  tererContentCoun
+00003c60: 7473 2e74 6573 745f 6765 745f 6772 6f75  ts.test_get_grou
+00003c70: 7065 645f 6d61 705f 636f 6e74 656e 7473  ped_map_contents
+00003c80: 4e29 0972 7e00 0000 727f 0000 0072 8000  N).r~...r....r..
+00003c90: 0000 7294 0000 0072 9b00 0000 729f 0000  ..r....r....r...
+00003ca0: 0072 a200 0000 72a4 0000 0072 a700 0000  .r....r....r....
+00003cb0: 722e 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
+00003cc0: 2f00 0000 7281 0000 00e0 0100 0073 0c00  /...r........s..
+00003cd0: 0000 0802 0876 0844 0843 081d 081a 7281  .....v.D.C....r.
+00003ce0: 0000 0072 5500 0000 7257 0000 0029 01da  ...rU...rW...)..
+00003cf0: 2641 4e59 434c 5553 5445 525f 4144 4449  &ANYCLUSTER_ADDI
+00003d00: 5449 4f4e 414c 5f47 524f 5550 5f42 595f  TIONAL_GROUP_BY_
+00003d10: 434f 4c55 4d4e 5363 0000 0000 0000 0000  COLUMNSc........
+00003d20: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+00003d30: 731c 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
+00003d40: 0284 005a 0364 0364 0484 005a 0464 0553  ...Z.d.d...Z.d.S
+00003d50: 0029 06da 2354 6573 744d 6170 436c 7573  .)..#TestMapClus
+00003d60: 7465 7265 7241 6c74 6572 6e61 7469 7665  tererAlternative
+00003d70: 5365 7474 696e 6773 6301 0000 0000 0000  Settingsc.......
+00003d80: 0000 0000 000a 0000 0009 0000 0043 0000  .............C..
+00003d90: 0073 6600 0000 6401 7d01 6700 7d02 7400  .sf...d.}.g.}.t.
+00003da0: 4400 5d54 7d03 7401 4400 5d4a 7d04 7402  D.]T}.t.D.]J}.t.
+00003db0: 7403 7404 7405 6604 4400 5d38 7d05 7c00  t.t.t.f.D.]8}.|.
+00003dc0: a006 7c04 7c01 7c03 7c02 a104 7d06 7407  ..|.|.|.|...}.t.
+00003dd0: 7c06 7408 6402 8d02 7d07 7c07 a009 a100  |.t.d...}.|.....
+00003de0: 7d08 6403 7d09 7c00 a00a 7c08 7c09 a102  }.d.}.|...|.|...
+00003df0: 0100 7124 7114 710c 6400 5300 2904 4e72  ..q$q.q.d.S.).Nr
+00003e00: 6a00 0000 7289 0000 007a 4c2c 204d 494e  j...r....zL, MIN
+00003e10: 2872 6174 696e 673a 3a56 4152 4348 4152  (rating::VARCHAR
+00003e20: 2920 4153 2072 6174 696e 672c 204d 494e  ) AS rating, MIN
+00003e30: 286c 6173 745f 7265 6e65 7761 6c3a 3a56  (last_renewal::V
+00003e40: 4152 4348 4152 2920 4153 206c 6173 745f  ARCHAR) AS last_
+00003e50: 7265 6e65 7761 6c29 0b72 0b00 0000 720e  renewal).r....r.
+00003e60: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00003e70: 0000 7214 0000 0072 2000 0000 7209 0000  ..r....r ...r...
+00003e80: 0072 8e00 0000 5a26 6765 745f 6164 6469  .r....Z&get_addi
+00003e90: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
+00003ea0: 636f 6c75 6d6e 735f 7374 7269 6e67 7221  columns_stringr!
+00003eb0: 0000 0029 0a72 2700 0000 722c 0000 0072  ...).r'...r,...r
+00003ec0: 2b00 0000 7228 0000 0072 2900 0000 7238  +...r(...r)...r8
+00003ed0: 0000 0072 2200 0000 722d 0000 005a 0e63  ...r"...r-...Z.c
+00003ee0: 6f6c 756d 6e73 5f73 7472 696e 6772 6800  olumns_stringrh.
+00003ef0: 0000 722e 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+00003f00: 00da 2b74 6573 745f 6765 745f 6164 6469  ..+test_get_addi
+00003f10: 7469 6f6e 616c 5f67 726f 7570 5f62 795f  tional_group_by_
+00003f20: 636f 6c75 6d6e 735f 7374 7269 6e67 4003  columns_string@.
+00003f30: 0000 7314 0000 0000 0204 0104 0208 0108  ..s.............
+00003f40: 0210 0210 020c 0208 0204 017a 4f54 6573  ...........zOTes
+00003f50: 744d 6170 436c 7573 7465 7265 7241 6c74  tMapClustererAlt
+00003f60: 6572 6e61 7469 7665 5365 7474 696e 6773  ernativeSettings
+00003f70: 2e74 6573 745f 6765 745f 6164 6469 7469  .test_get_additi
+00003f80: 6f6e 616c 5f67 726f 7570 5f62 795f 636f  onal_group_by_co
+00003f90: 6c75 6d6e 735f 7374 7269 6e67 6301 0000  lumns_stringc...
+00003fa0: 0000 0000 0000 0000 000c 0000 000a 0000  ................
+00003fb0: 0043 0000 0073 be00 0000 6401 7d01 6700  .C...s....d.}.g.
+00003fc0: 7d02 7c00 a000 6402 6403 a102 0100 7c00  }.|...d.d.....|.
+00003fd0: a000 6404 6405 a102 0100 7c00 a001 7402  ..d.d.....|...t.
+00003fe0: 7403 6406 8302 a101 0100 7404 4400 5d84  t.d.......t.D.].
+00003ff0: 7d03 7405 4400 5d7a 7d04 7406 7407 7408  }.t.D.]z}.t.t.t.
+00004000: 7409 6604 4400 5d68 7d05 7c00 a00a 7c04  t.f.D.]h}.|...|.
+00004010: 7c01 7c03 7c02 a104 7d06 740b 7c06 740c  |.|.|...}.t.|.t.
+00004020: 6407 8d02 7d07 6408 7d08 7c07 a00d 7c05  d...}.d.}.|...|.
+00004030: 7c04 7c01 7c02 7c08 a105 7d09 7c04 740e  |.|.|.|...}.|.t.
+00004040: 6b02 724c 7c09 a00f a100 4400 5d20 5c02  k.rL|.....D.] \.
+00004050: 7d0a 7d0b 7c00 a010 6409 7c0b a102 0100  }.}.|...d.|.....
+00004060: 7c00 a010 640a 7c0b a102 0100 7192 714c  |...d.|.....q.qL
+00004070: 713c 7134 6400 5300 290b 4e72 6a00 0000  q<q4d.S.).Nrj...
+00004080: 728b 0000 0072 8200 0000 728c 0000 0072  r....r....r....r
+00004090: 8d00 0000 72a8 0000 0072 8900 0000 7254  ....r....r....rT
+000040a0: 0000 0072 5500 0000 7257 0000 0029 1172  ...rU...rW...).r
+000040b0: 8f00 0000 7235 0000 00da 0768 6173 6174  ....r5.....hasat
+000040c0: 7472 7205 0000 0072 0b00 0000 720e 0000  trr....r....r...
+000040d0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000040e0: 7214 0000 0072 2000 0000 7209 0000 0072  r....r ...r....r
+000040f0: 8e00 0000 72a5 0000 0072 0c00 0000 da05  ....r....r......
+00004100: 6974 656d 73da 0861 7373 6572 7449 6e29  items..assertIn)
+00004110: 0c72 2700 0000 722c 0000 0072 2b00 0000  .r'...r,...r+...
+00004120: 7228 0000 0072 2900 0000 7238 0000 0072  r(...r)...r8...r
+00004130: 2200 0000 722d 0000 0072 a600 0000 7291  "...r-...r....r.
+00004140: 0000 00da 0961 6767 7265 6761 7465 da04  .....aggregate..
+00004150: 6461 7461 722e 0000 0072 2e00 0000 722f  datar....r....r/
+00004160: 0000 00da 3074 6573 745f 6765 745f 6772  ....0test_get_gr
+00004170: 6f75 7065 645f 6d61 705f 636f 6e74 656e  ouped_map_conten
+00004180: 7473 5f61 6464 6974 696f 6e61 6c5f 636f  ts_additional_co
+00004190: 6c75 6d6e 7354 0300 0073 2000 0000 0002  lumnsT...s .....
+000041a0: 0401 0402 0c01 0c02 1002 0801 0802 1002  ................
+000041b0: 1002 0c02 0402 1202 0802 1002 0c01 7a54  ..............zT
+000041c0: 5465 7374 4d61 7043 6c75 7374 6572 6572  TestMapClusterer
+000041d0: 416c 7465 726e 6174 6976 6553 6574 7469  AlternativeSetti
+000041e0: 6e67 732e 7465 7374 5f67 6574 5f67 726f  ngs.test_get_gro
+000041f0: 7570 6564 5f6d 6170 5f63 6f6e 7465 6e74  uped_map_content
+00004200: 735f 6164 6469 7469 6f6e 616c 5f63 6f6c  s_additional_col
+00004210: 756d 6e73 4e29 0572 7e00 0000 727f 0000  umnsN).r~...r...
+00004220: 0072 8000 0000 72aa 0000 0072 b000 0000  .r....r....r....
+00004230: 722e 0000 0072 2e00 0000 722e 0000 0072  r....r....r....r
+00004240: 2f00 0000 72a9 0000 003c 0300 0073 0400  /...r....<...s..
+00004250: 0000 0804 0814 72a9 0000 0029 27da 0b64  ......r....)'..d
+00004260: 6a61 6e67 6f2e 7465 7374 7202 0000 0072  jango.testr....r
+00004270: 0300 0000 7204 0000 00da 0b64 6a61 6e67  ....r......djang
+00004280: 6f2e 636f 6e66 7205 0000 00da 1764 6a61  o.confr......dja
+00004290: 6e67 6f2e 636f 6e74 7269 622e 6769 732e  ngo.contrib.gis.
+000042a0: 6765 6f73 7206 0000 00da 1764 6a61 6e67  geosr......djang
+000042b0: 6f2e 636f 6e74 7269 622e 6769 732e 6764  o.contrib.gis.gd
+000042c0: 616c 7207 0000 0072 0800 0000 5a17 616e  alr....r....Z.an
+000042d0: 7963 6c75 7374 6572 2e4d 6170 436c 7573  ycluster.MapClus
+000042e0: 7465 7265 7272 0900 0000 da0a 616e 7963  tererr......anyc
+000042f0: 6c75 7374 6572 720a 0000 00da 1661 6e79  lusterr......any
+00004300: 636c 7573 7465 722e 6465 6669 6e69 7469  cluster.definiti
+00004310: 6f6e 7372 0b00 0000 720c 0000 0072 0d00  onsr....r....r..
+00004320: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00004330: 005a 1761 6e79 636c 7573 7465 722e 7465  .Z.anycluster.te
+00004340: 7374 732e 636f 6d6d 6f6e 7211 0000 0072  sts.commonr....r
+00004350: 1200 0000 7213 0000 0072 1400 0000 5a17  ....r....r....Z.
+00004360: 616e 7963 6c75 7374 6572 2e74 6573 7473  anycluster.tests
+00004370: 2e6d 6978 696e 7372 1500 0000 7216 0000  .mixinsr....r...
+00004380: 0072 1700 0000 5a0d 616e 796d 6170 2e6d  .r....Z.anymap.m
+00004390: 6f64 656c 7372 1800 0000 7246 0000 0072  odelsr....rF...r
+000043a0: 1f00 0000 728e 0000 0072 1b00 0000 7281  ....r....r....r.
+000043b0: 0000 0072 a900 0000 722e 0000 0072 2e00  ...r....r....r..
+000043c0: 0000 722e 0000 0072 2f00 0000 da08 3c6d  ..r....r/.....<m
+000043d0: 6f64 756c 653e 0100 0000 732a 0000 0014  odule>....s*....
+000043e0: 010c 010c 0110 010c 010c 0220 0218 0114  ........... ....
+000043f0: 020c 0208 0204 0104 0214 7f00 7f00 7f00  ................
+00004400: 4f14 7f00 7f00 5e0c 01                   O.....^..
```

### Comparing `anycluster-2.3.3/anycluster/tests/common.py` & `anycluster-2.3.4/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/mixins.py` & `anycluster-2.3.4/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/test_ClusterCache.py` & `anycluster-2.3.4/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/test_FilterComposer.py` & `anycluster-2.3.4/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/anycluster/tests/test_MapClusterer.py` & `anycluster-2.3.4/anycluster/tests/test_MapClusterer.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,45 +601,46 @@
 
         zoom = 10
         geometry_type = GEOMETRY_TYPE_VIEWPORT
         clustertype = CLUSTER_TYPE_KMEANS
 
         
         filters = []
+        modulation_filters = []
 
         cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
         map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
 
         geojson = GEOJSON_RECTANGLE
 
         geometries_for_counting = map_clusterer.get_geometries_for_counting(geojson, geometry_type, zoom)
 
-        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, modulation_filters)
         self.assertEqual(count, 0)
 
         self.create_point('name 1', 'stone')
         
-        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, modulation_filters)
         self.assertEqual(count, 1)
 
         self.create_point('name 2', 'flower')
 
-        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, modulation_filters)
         self.assertEqual(count, 2)
 
 
         filters = [
             {
                 'column': 'style',
                 'value': 'stone',
                 'operator': '=',
             }
         ]
 
-        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, modulation_filters)
         self.assertEqual(count, 1)
 
         filters = [
             {
                 'column': 'style',
                 'value': 'stone',
                 'operator': '=',
@@ -648,27 +649,93 @@
                 'column': 'style',
                 'value': 'flower',
                 'operator': '=',
                 'logicalOperator': 'OR',
             }
         ]
 
-        count = map_clusterer.query_map_content_count(geometries_for_counting, filters)
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, modulation_filters)
         self.assertEqual(count, 2)
 
         gardens = Gardens.objects.all()
         for garden in gardens:
             garden.delete()
 
-
         gardens = Gardens.objects.all()
 
         self.assertEqual(gardens.count(), 0)
 
 
+    def test_query_map_content_count_with_modulations(self):
+
+        zoom = 10
+        geometry_type = GEOMETRY_TYPE_VIEWPORT
+        clustertype = CLUSTER_TYPE_KMEANS
+
+        filters = [
+            {
+                'column': 'style',
+                'value': 'stone',
+                'operator': '=',
+            },
+            {
+                'column': 'style',
+                'value': 'flower',
+                'operator': '=',
+                'logicalOperator': 'OR',
+            }
+        ]
+
+        cluster_cache = self.get_cluster_cache(geometry_type, zoom, clustertype, filters)
+        map_clusterer = MapClusterer(cluster_cache, grid_size=TEST_GRID_SIZE)
+
+        geojson = GEOJSON_RECTANGLE
+
+        geometries_for_counting = map_clusterer.get_geometries_for_counting(geojson, geometry_type, zoom)
+
+
+        stone_modulation = [{
+            'column': 'style',
+            'value': 'stone',
+            'operator': '=',
+        }]
+
+
+        garden_1 = self.create_point('name 1', 'stone')
+        garden_2 =  self.create_point('name 2', 'flower')
+        garden_3 = self.create_point('name 3', 'stone')
+        garden_4 = self.create_point('name 4', 'stone')
+        garden_5 = self.create_point('name 5', 'stone')
+        garden_6 = self.create_point('name 6', 'stone')
+
+        garden_1.free_entrance = True
+        garden_1.save()
+        garden_3.free_entrance = True
+        garden_3.save()
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, stone_modulation)
+        self.assertEqual(count, 5)
+
+        stone_free_modulation = [
+            {
+                'column': 'style',
+                'value': 'stone',
+                'operator': '=',
+            },
+            {
+                'column': 'free_entrance',
+                'value': True,
+                'operator': '=',
+                'logicalOperator': 'AND',
+            },
+        ]
+
+        count = map_clusterer.query_map_content_count(geometries_for_counting, filters, stone_free_modulation)
+        self.assertEqual(count, 2)
+
     def test_get_geometries_for_counting(self):
         
         zoom = 10
         
         for clustertype in CLUSTER_TYPES:
             for geometry_type in GEOMETRY_TYPES:
```

### Comparing `anycluster-2.3.3/anycluster.egg-info/PKG-INFO` & `anycluster-2.3.4/anycluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.3
+Version: 2.3.4
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.3/anycluster.egg-info/SOURCES.txt` & `anycluster-2.3.4/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.3/setup.py` & `anycluster-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.3.3',
+    version='2.3.4',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

