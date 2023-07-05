# Comparing `tmp/forecastmanager-0.0.3.tar.gz` & `tmp/forecastmanager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.3.tar", last modified: Mon Jun 19 08:57:00 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.4.tar", last modified: Wed Jul  5 08:41:59 2023, max compression
```

## Comparing `forecastmanager-0.0.3.tar` & `forecastmanager-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/query_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:57:00.774028 forecastmanager-0.0.3/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 08:57:00.000000 forecastmanager-0.0.3/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 08:56:42.000000 forecastmanager-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 08:57:00.778028 forecastmanager-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.600008 forecastmanager-0.0.4/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.600008 forecastmanager-0.0.4/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.600008 forecastmanager-0.0.4/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.600008 forecastmanager-0.0.4/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.596008 forecastmanager-0.0.4/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.596008 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/static/forecastmanager/js/helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.596008 forecastmanager-0.0.4/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/load_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/query_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:41:59.600008 forecastmanager-0.0.4/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 08:41:59.000000 forecastmanager-0.0.4/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-05 08:41:59.000000 forecastmanager-0.0.4/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:41:59.000000 forecastmanager-0.0.4/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-05 08:41:59.000000 forecastmanager-0.0.4/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 08:41:59.000000 forecastmanager-0.0.4/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 08:41:45.000000 forecastmanager-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-05 08:41:59.604008 forecastmanager-0.0.4/setup.cfg
```

### Comparing `forecastmanager-0.0.3/PKG-INFO` & `forecastmanager-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -12,9 +12,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `forecastmanager-0.0.3/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.4/forecastmanager/management/commands/generate_forecast.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.core.management.base import BaseCommand
 
 import pandas as pd
 import json
 import requests
 
 from wagtailgeowidget.helpers import geosgeometry_str_to_struct
-from forecastmanager.models import City,Forecast, ConditionCategory
+from forecastmanager.models import City,Forecast
 
 
 # Define the base URL for the Met Norway API
 BASE_URL = "https://api.met.no/weatherapi/locationforecast/2.0/compact"
 headers = {
   'User-Agent':'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Mobile Safari/537.36'
 }
@@ -60,25 +60,20 @@
                 df.set_index('time', inplace=True)
 
                 # Define a function to extract the required values from a group
                 def extract_values(group):
                     # Extract the minimum and maximum values of air temperature, wind speed, and wind direction
                     min_temp = group['data.instant.details.air_temperature'].min()
                     max_temp = group['data.instant.details.air_temperature'].max()
-                    wind_speed = group['data.instant.details.wind_speed'].mean()
-                    wind_dir = group['data.instant.details.wind_from_direction'].mean()
                     # Extract the value of next_12_hours summary
                     next_12_hours = group['data.next_12_hours.summary.symbol_code'].iloc[0]
                     # Create a dictionary of the extracted values
-                    values = {'min_temp': min_temp, 'max_temp': max_temp, 'wind_speed': wind_speed,
-                            'wind_dir': wind_dir, 
+                    values = {'min_temp': min_temp, 'max_temp': max_temp, 
                             'next_12_hours': next_12_hours}
                     return pd.Series(values, index=['min_temp', 'max_temp', 
-                                                    'wind_speed', 
-                                                    'wind_dir', 
                                                     'next_12_hours'])
 
                 # Group the DataFrame by date and apply the extract_values() function to each group
                 grouped = df.groupby(pd.Grouper(freq='D')).apply(extract_values)
                 grouped = grouped.dropna()
 
                 # Get the name of the parent from the first column
@@ -86,36 +81,32 @@
                 # Try to get an existing parent with the same name, or create a new one
                 city = City.objects.get(name=parent_name)
                 
                 for index, row in grouped.iterrows():
                     time = index.to_pydatetime()
                     min_temp = row['min_temp']
                     max_temp = row['max_temp']
-                    wind_speed = row['wind_speed']
-                    wind_dir = row['wind_dir']
 
                     # Create or update the child object with the parent and the name from the second column
                     # prioritize condition for the next 1 hour 
                     if 'next_1_hours' in row:
-                        condition = ConditionCategory.objects.get(short_name=row['next_1_hours']) 
+                        condition = row['next_1_hours'].split("_")[0]
                     elif 'next_6_hours' in row:
-                        condition = ConditionCategory.objects.get(short_name=row['next_6_hours']) 
+                        condition = row['next_6_hours'].split("_")[0]
                     else:
-                        condition = ConditionCategory.objects.get(short_name=row['next_12_hours']) 
+                        condition = row['next_12_hours'].split("_")[0]
 
                     # use update_or_create to update existing data
                     # and create new ones if the data does not exist
                     obj, created = Forecast.objects.update_or_create(
                         forecast_date=time,
                         city=city, 
                         defaults={
                             'min_temp': min_temp,
                             'max_temp': max_temp,
-                            'wind_speed': wind_speed,
-                            'wind_direction': wind_dir,
                             'condition': condition
                         }
                     )
 
             else:
                 # Handle errors
                 print(f"Error fetching weather data for ({lat}, {lon}): {response.status_code}")
```

### Comparing `forecastmanager-0.0.3/forecastmanager/site_settings.py` & `forecastmanager-0.0.4/forecastmanager/site_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.utils.translation import gettext_lazy as _
 from wagtail.admin.panels import (
     FieldPanel,
     TabbedInterface,
     ObjectList,
 )
 @register_setting
-class Setting(BaseSiteSetting):
+class ForecastSetting(BaseSiteSetting):
     enable_auto_forecast = models.BooleanField(
         default=True,
         verbose_name=_('Enable automated forecasts')
     )
 
     TEMPERATURE_UNITS = (
         ("celsius", "°C"),
```

### Comparing `forecastmanager-0.0.3/forecastmanager/templates/forecastmanager/query_forecast.html` & `forecastmanager-0.0.4/forecastmanager/templates/forecastmanager/query_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.3/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.4/forecastmanager/wagtail_hooks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from django.urls import path, include, reverse
 from wagtail.admin.menu import MenuItem
 from wagtail import hooks
 # from . import urls
 from django.utils.html import format_html
 from django.templatetags.static import static
-from forecastmanager.models import City, ConditionCategory
-from forecastmanager.site_settings import Setting 
+from forecastmanager.models import City, DailyWeather
+from forecastmanager.site_settings import ForecastSetting 
 from django.utils.translation import gettext_lazy as _
 from django.urls import path
 from django.urls import re_path
-from forecastmanager.views import add_forecast, save_data, get_data
+from forecastmanager.views import add_forecast, save_data,get_forecast
 from wagtail.contrib.modeladmin.options import (
     ModelAdmin, 
     modeladmin_register,
     ModelAdminGroup
 )
 
 
@@ -23,74 +23,77 @@
     Registers forecast urls in the wagtail admin.
     """
     return [
         # path(
         #     "forecast/",
         #     include((urls, "forecast"), namespace="forecast_admin"),
         # ),
+        path("load_forecast/", get_forecast, name="load_forecast"),
         path("add_forecast/", add_forecast, name="add_forecast"),
         path('save-data/', save_data, name='save_data'),
-        re_path(r'^get-data/$', get_data, name='get_data'),
-
         
     ]
 
 
-@hooks.register("insert_global_admin_css")
-def insert_global_admin_css():
-    return format_html(
-        '<link rel="stylesheet" type="text/css" href="{}">',
-        static("css/admin.css"),
-    )
-
-class SettingsAdmin(ModelAdmin):
-    model = Setting
+class ForecastSettingAdmin(ModelAdmin):
+    model = ForecastSetting
     menu_label = 'Settings'
     menu_icon = 'cog'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
 class CitiesAdmin(ModelAdmin):
     model = City
     menu_label = 'Cities'
-    menu_icon = 'cog'
+    menu_icon = 'site'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
-class ConditionCategoryAdmin(ModelAdmin):
-    model = ConditionCategory
-    menu_label = 'Weather Conditions'
-    menu_icon = 'cog'
+class DailyWeatherAdmin(ModelAdmin):
+    model = DailyWeather
+    menu_label = 'Daily Weather'
+    menu_icon = 'site'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
+
+# class ConditionCategoryAdmin(ModelAdmin):
+#     model = ConditionCategory
+#     menu_label = 'Weather Conditions'
+#     menu_icon = 'cog'
+#     add_to_settings_menu = False
+#     exclude_from_explorer = False
+
 class CityForecastGroup(ModelAdminGroup):
     menu_label = 'City Forecast'
     menu_icon = 'table'  # change as required
     menu_order = 200  # will put in 3rd place (000 being 1st, 100 2nd)
-    items = (CitiesAdmin, ConditionCategoryAdmin)
+    items = (CitiesAdmin, DailyWeatherAdmin)
 
     def get_submenu_items(self):
         menu_items = []
         item_order = 1
         for modeladmin in self.modeladmin_instances:
             menu_items.append(modeladmin.get_menu_item(order=item_order))
             item_order += 1
 
             # append raster upload link
-        upload_menu_item = MenuItem(label="Forecasts", url=reverse("add_forecast"), icon_name="cog")
-
-        menu_items.append(upload_menu_item)
+        add_forecast_item = MenuItem(label="Add Forecasts", url=reverse("add_forecast"), icon_name="plus")
+        load_forecast_item = MenuItem(label="Load Forecasts", url=reverse("load_forecast"), icon_name="view")
+        
+        menu_items.append(add_forecast_item)
+        menu_items.append(load_forecast_item)
 
         try:
             settings_url = reverse(
                 "wagtailsettings:edit",
-                args=[Setting._meta.app_label, Setting._meta.model_name, ],
+                args=[ForecastSetting._meta.app_label, ForecastSetting._meta.model_name, ],
             )
             gm_settings_menu = MenuItem(label=_("Settings"), url=settings_url, icon_name="cog")
             menu_items.append(gm_settings_menu)
         except Exception:
             pass
 
         return menu_items
+    
 
-modeladmin_register(CityForecastGroup)
+modeladmin_register(CityForecastGroup)
```

### Comparing `forecastmanager-0.0.3/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.4/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -12,9 +12,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `forecastmanager-0.0.3/setup.cfg` & `forecastmanager-0.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.3
+version = 0.0.4
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
@@ -19,17 +19,18 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 include_package_data = true
-python_requires = >=3.9
+python_requires = >=3.8
 install_requires = 
 	wagtail>=4.2.2
 	wagtailgeowidget>=7.0.0
 	pandas>=2.0.2
+	psycopg2-binary>=2.9.5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

