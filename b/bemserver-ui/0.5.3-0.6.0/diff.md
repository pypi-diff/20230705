# Comparing `tmp/bemserver-ui-0.5.3.tar.gz` & `tmp/bemserver-ui-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-ui-0.5.3.tar", last modified: Fri Jun 16 08:46:45 2023, max compression
+gzip compressed data, was "bemserver-ui-0.6.0.tar", last modified: Wed Jul  5 08:22:06 2023, max compression
```

## Comparing `bemserver-ui-0.5.3.tar` & `bemserver-ui-0.6.0.tar`

### file list

```diff
@@ -1,317 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/campaign_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/flask_es6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/jinja_custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-areas.json
--rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-full.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/weather_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/accordionList.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/dropZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/eventLevel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/filterSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/flash.js
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/itemsCount.js
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/modalConfirm.js
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/spinner.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/tree.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/flashTimer.js
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/formController.js
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/sidebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/array.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/dict.js
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/fetcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/flaskES6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/time.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/weather.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/list.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
--rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
--rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/dragndrop.css
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/main.css
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/tree.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/campaigns/selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_services.html
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/user_group_available.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_for_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/structural_element_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/ts_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/flash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/partners.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/degree_days.html
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/energy_consumption.html
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/weather.html
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/setup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/explore.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/completeness.html
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/semantic_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/campaigns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/weather_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.219583 bemserver-ui-0.6.0/bemserver_ui/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/campaign_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/flask_es6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/jinja_custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.219583 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-areas.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-full.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/weather_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/accordionList.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/dropZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/eventLevel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/filterSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/flash.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/itemsCount.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/spinner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/tree.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/flashTimer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/formController.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/sidebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/dict.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/fetcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/time.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/weather.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/list.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/
+-rw-r--r--   0 runner    (1001) docker     (123)    28668 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)    33076 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36298 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19413 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/dragndrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/signin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/tree.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_services.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/user_group_available.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_for_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/structural_element_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/ts_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/partners.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/degree_days.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/energy_consumption.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/weather.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/setup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/skeleton.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/start.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/stats.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/explore.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/completeness.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/campaigns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/weather_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/tox.ini
```

### Comparing `bemserver-ui-0.5.3/LICENSE` & `bemserver-ui-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/PKG-INFO` & `bemserver-ui-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.3
+Version: 0.6.0
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,16 @@
         Is API published through SSL?
     **BEMSERVER_API_AUTH_METHOD = "http_basic"**
         API authentication method
     **BEMSERVER_UI_TIMEZONE_NAME = "UTC"**
         Default application timezone name, when not overrided campaign timezone
     **BEMSERVER_UI_NOTIFICATION_UPDATER_DELAY = 60000**
         Delay, in seconds, between each check of new notifications
+    **BEMSERVER_UI_USER_GUIDE_URL = https://bemserver-docs.readthedocs.io/en/latest/user_guide.html**
+        User guide URL
     *(optional)* **BEMSERVER_UI_PARTNERS_FILE = None**
         Absolute path of json file that describes the project's partners
 
         Example of ``BEMSERVER_UI_PARTNERS_FILE`` file structure::
 
             [
                 {
```

### Comparing `bemserver-ui-0.5.3/README.rst` & `bemserver-ui-0.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         Is API published through SSL?
     **BEMSERVER_API_AUTH_METHOD = "http_basic"**
         API authentication method
     **BEMSERVER_UI_TIMEZONE_NAME = "UTC"**
         Default application timezone name, when not overrided campaign timezone
     **BEMSERVER_UI_NOTIFICATION_UPDATER_DELAY = 60000**
         Delay, in seconds, between each check of new notifications
+    **BEMSERVER_UI_USER_GUIDE_URL = https://bemserver-docs.readthedocs.io/en/latest/user_guide.html**
+        User guide URL
     *(optional)* **BEMSERVER_UI_PARTNERS_FILE = None**
         Absolute path of json file that describes the project's partners
 
         Example of ``BEMSERVER_UI_PARTNERS_FILE`` file structure::
 
             [
                 {
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 
 from . import extensions
 from . import internal_api
 from . import views
 
 
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 
 def create_app(config_override=None):
     """Create application"""
     app = flask.Flask(__name__)
     app.config.from_object("bemserver_ui.settings.Config")
     app.config.from_envvar("BEMSERVER_UI_SETTINGS_FILE", silent=True)
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/common/time.py` & `bemserver-ui-0.6.0/bemserver_ui/common/time.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/common/tree.py` & `bemserver-ui-0.6.0/bemserver_ui/common/tree.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/api_client.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/auth.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/campaign_context.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/campaign_context.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/error_handlers.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/error_handlers.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/flask_es6.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/flask_es6.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/jinja_custom_filters.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/jinja_custom_filters.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/partners.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/partners.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/plugins.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/plugins.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-areas.json` & `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-areas.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-full.json` & `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-full.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones.py` & `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/completeness.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/degree_days.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/energy_consumption.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/campaign_scopes.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/campaigns.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/events.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/notifications.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/consumption.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/production.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/production.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/weather.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/weather.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/cleanup.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/missing_data.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/outlier_data.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/weather_data.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/weather_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/structural_elements.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/data.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,21 @@
             dt_start.isoformat(),
             dt_end.isoformat(),
             data_state_id,
             ts_ids,
             timezone=tz_name,
         )
 
-    return flask.jsonify(ts_data_resp.data)
+    ts_data = ts_data_resp.data
+    # Ensure each timeseries is in returned result, especially when not aggregated.
+    for ts_id in ts_ids:
+        if str(ts_id) not in ts_data:
+            ts_data[str(ts_id)] = {}
+
+    return flask.jsonify(ts_data)
 
 
 @blp.route("/delete_data", methods=["POST"])
 @auth.signin_required
 @ensure_campaign_context
 def delete_data():
     tz_name = flask.request.json["timezone"]
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/timeseries.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/user_groups.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/internal_api/users.py` & `bemserver-ui-0.6.0/bemserver_ui/internal_api/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-ico.svg` & `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-ico.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-min.svg` & `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-min.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.ico` & `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.ico`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.svg` & `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/app.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/app.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -7,67 +7,62 @@
 import {
     Sidebar
 } from "./modules/sidebar.js";
 import {
     FormController
 } from "./modules/formController.js";
 import {
-    CampaignSelectorView
-} from "./modules/views/campaigns/selector.js";
-import {
     flaskEndpoints
 } from "./modules/flaskES6-endpoints.js";
 import {
     FlashTimer
 } from "./modules/flashTimer.js";
 import {
     NotificationUpdater
 } from "./modules/notifications.js";
 
 
 // TODO: how can app instance be accessible from any module?
 // TODO: when app instance is accessible by any other module, put flaskES6 instance inside
 // TODO: manage flash messages in through this app class?
+// TODO: campaignContext defined here is not used for now...
 
 
 const campaignContextQueryArgName = "campaign_ctxt";
 const flaskES6 = new FlaskES6(flaskEndpoints, campaignContextQueryArgName);
 
 
 export class App {
 
     #notifUpdatedDelay = 60000;
     #campaignContext = {};
 
-    #campaignSelector = new CampaignSelectorView();
     #sidebar = new Sidebar();
     #formCtrl = new FormController();
     #flashTimer = new FlashTimer();
     #notifUpdater = null;
 
     constructor(options = {}) {
         this.#loadOptions(options);
 
         this.#sidebar = new Sidebar();
-        this.#campaignSelector = new CampaignSelectorView();
         this.#formCtrl = new FormController();
         this.#flashTimer = new FlashTimer();
         this.#notifUpdater = new NotificationUpdater({
             delay: this.#notifUpdatedDelay
         });
     }
 
     #loadOptions(options = {}) {
         this.#notifUpdatedDelay = options.notificationUpdaterDelay || 60000;
         this.#campaignContext = options.campaignContext || {};
     }
 
     mount() {
         this.#sidebar.refresh();
-        this.#campaignSelector.hide();
         this.#formCtrl.bind();
         this.#flashTimer.bind();
         this.#notifUpdater.refresh();
     }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/accordionList.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/accordionList.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
-import "https://cdn.jsdelivr.net/npm/echarts@5.4.1/dist/echarts.min.js";
+import "https://cdn.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js";
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 import {
     TimeDisplay
-} from "../../tools/time.js";
+} from "/static/scripts/modules/tools/time.js";
 
 
 export class TimeseriesChartCompleteness extends HTMLDivElement {
 
     #chart = null;
 
     #initOptions = {
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-import "https://cdn.jsdelivr.net/npm/echarts@5.4.1/dist/echarts.min.js";
+import "https://cdn.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js";
 import {
     Parser
 } from "/static/scripts/modules/tools/parser.js";
 
 
 export class TimeseriesChartDegreeDays extends HTMLDivElement {
 
@@ -20,24 +20,21 @@
             left: "center",
             text: this.#defaultTitle,
             subtextStyle: {
                 fontSize: 14,
             },
         },
         grid: {
-            left: "3%",
-            right: "5%",
+            left: 20,
+            right: 20,
             bottom: 90,
             containLabel: true,
         },
         toolbox: {
             feature: {
-                dataZoom: {
-                    yAxisIndex: "none",
-                },
                 dataView: {
                     readOnly: true,
                     buttonColor: "#95c11a",
                 },
                 saveAsImage: {},
             },
         },
@@ -45,27 +42,27 @@
             trigger: "axis",
             axisPointer: {
                 type: "shadow",
             },
         },
         legend: {
             type: "scroll",
-            bottom: 10,
+            bottom: 0,
         },
         dataZoom: [{
             type: "slider",
             bottom: 50,
+        }, {
+            type: "inside",
         }, ],
         xAxis: [{
             type: "time",
         }, ],
         yAxis: [{
             type: "value",
-            nameLocation: "middle",
-            axisLabel: {},
         }, ],
         series: [],
         useUTC: false,
     };
 
     #degreeDayTypeColors = {
         "heating": "#ee6666",
@@ -241,14 +238,16 @@
         options.toolbox[0].feature.dataView.optionToContent = (opt) => {
             return this.#optionToContent(opt, unit, timeFormat);
         };
         options.tooltip[0].formatter = (params) => {
             return this.#tooltipFormatter(params, unit, timeFormat);
         };
 
+        options.yAxis[0].name = unit;
+
         options.series.length = 0;
         if (!this.#compareMode) {
             options.series.push({
                 id: `${degreeDaysType}-${degreeDaysBase}`,
                 name: `${degreeDaysType} degree days (base ${degreeDaysBase.toString()}${degreeDaysBaseUnit ? ` ${degreeDaysBaseUnit}`: ""})`,
                 type: "bar",
                 data: Object.entries(degreeDaysData).map(([timestamp, value]) => {
@@ -275,19 +274,14 @@
                     emphasis: {
                         focus: "series",
                     },
                 };
             });
         }
 
-        options.yAxis[0].data = options.series.map((serie) => {
-            return serie.name;
-        });
-        options.yAxis[0].axisLabel.formatter = `{value} ${unit}`;
-
         // Fix for bug, see: https://github.com/apache/incubator-echarts/issues/6202
         this.#chart.clear();
 
         this.#chart.setOption(options);
     }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-import "https://cdn.jsdelivr.net/npm/echarts@5.4.1/dist/echarts.min.js";
+import "https://cdn.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js";
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 
 
 export class TimeseriesChartEnergyConsumption extends HTMLDivElement {
 
     #chart = null;
 
     #initOptions = {
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -216,15 +216,15 @@
 
         if (applyOption) {
             this.#setChartOptions();
         }
     }
 
     #prepareSeriesData(data) {
-        return Object.entries(data).map(([timestamp, value]) => {
+        return Object.entries(data || {}).map(([timestamp, value]) => {
             return [timestamp, Parser.parseFloatOrDefault(value, Number.NaN, 2)];
         });
     }
 
     #optionToContent(opt) {
         let mainContainerElmt = document.createElement("div");
         mainContainerElmt.classList.add("m-2", "me-3");
@@ -330,17 +330,15 @@
         // TODO: keep dataZoom values?
 
         this.#chart.setOption(this.#chartOpts);
     }
 
     addSeries(seriesParams, data = null) {
         if (!this.#hasSeries(seriesParams.id)) {
-            if (data != null) {
-                seriesParams.data = this.#prepareSeriesData(data);
-            }
+            seriesParams.data = this.#prepareSeriesData(data);
             this.#chartOpts.legend[seriesParams.yAxisIndex].data.push(seriesParams.name);
             this.#chartOpts.series.push(seriesParams);
 
             if (this.#chartOpts.series.length > 0) {
                 this.#hideNoData();
             }
 
@@ -422,18 +420,15 @@
     }
 
     updateSeriesData(id, data, options = {
         aggregation: null
     }) {
         let seriesIndex = this.#getSeriesIndex(id);
         if (seriesIndex != -1) {
-            if (data != null) {
-                this.#chartOpts.series[seriesIndex].data = this.#prepareSeriesData(data);
-            }
-            this.#chartOpts.series[seriesIndex].visible = true;
+            this.#chartOpts.series[seriesIndex].data = this.#prepareSeriesData(data);
             this.#chartOpts.series[seriesIndex].aggregation = options.aggregation;
 
             this.#setChartOptions();
         }
     }
 
     toggleSeriesVisibility(id) {
@@ -471,15 +466,17 @@
             this.#updateLegend();
 
             this.#setChartOptions();
         }
     }
 
     clear() {
+        // Fix for bug, see: https://github.com/apache/incubator-echarts/issues/6202
         this.#chart.clear();
+
         this.#chartOpts.series = [];
         for (let leg of this.#chartOpts.legend) {
             leg.data = [];
             leg.selected = {};
         }
         this.#updateYAxisName();
         this.#updateLegend();
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-import "https://cdn.jsdelivr.net/npm/echarts@5.4.1/dist/echarts.min.js";
+import "https://cdn.jsdelivr.net/npm/echarts@5.4.2/dist/echarts.min.js";
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 
 
 export class TimeseriesChartWeather extends HTMLDivElement {
 
     #chart = null;
 
     #initOptions = {
@@ -16,43 +16,44 @@
 
     #defaultOptions = {
         title: {
             left: "center",
             text: "",
         },
         grid: {
-            left: "3%",
-            right: "5%",
+            left: 20,
+            right: 20,
+            top: 70,
             bottom: 90,
             containLabel: true,
         },
         toolbox: {
             feature: {
                 myTSInfo: {
                     show: true,
                     title: "Weather parameters timeseries",
-                    icon: "path://M 12 2 C 6.4771525 2 2 6.4771525 2 12 C 2 17.522847 6.4771525 22 12 22 C 17.522847 22 22 17.522847 22 12 C 22 6.4771525 17.522847 2 12 2 z M 12 4 C 16.418278 4 20 7.581722 20 12 C 20 16.418278 16.418278 20 12 20 C 7.581722 20 4 16.418278 4 12 C 4 7.581722 7.581722 4 12 4 z M 11 6 L 11 8 L 13 8 L 13 6 L 11 6 z M 11 9 L 11 17 L 13 17 L 13 9 L 11 9 z",
-                    onclick: function() {
+                    icon: "path://m9.708 6.075-3.024.379-.108.502.595.108c.387.093.464.232.38.619l-.975 4.577c-.255 1.183.14 1.74 1.067 1.74.72 0 1.554-.332 1.933-.789l.116-.549c-.263.232-.65.325-.905.325-.363 0-.494-.255-.402-.704l1.323-6.208Zm.091-2.755a1.32 1.32 0 1 1-2.64 0 1.32 1.32 0 0 1 2.64 0Z",
+                    onclick: () => {
                         this.#showTSInfo();
                     },
                 },
-                dataZoom: {
-                    yAxisIndex: "none",
-                },
                 dataView: {
                     readOnly: true,
                     buttonColor: "#95c11a",
                 },
                 saveAsImage: {},
             },
         },
         tooltip: {
             trigger: "axis",
             axisPointer: {
-                type: "shadow",
+                type: "cross",
+            },
+            valueFormatter: (value) => {
+                return Parser.parseFloatOrDefault(value, Number.NaN, 2);
             },
         },
         legend: [{
             data: [],
             width: "45%",
             bottom: 0,
             left: 0,
@@ -63,28 +64,28 @@
             bottom: 0,
             right: 0,
             type: "scroll",
         }],
         dataZoom: [{
             type: "slider",
             bottom: 50,
+        }, {
+            type: "inside",
         }, ],
         xAxis: [{
             type: "time",
         }, ],
         yAxis: [{
             type: "value",
-            nameLocation: "middle",
-            axisLabel: {},
             position: "left",
+            scale: true,
         }, {
             type: "value",
-            nameLocation: "middle",
-            axisLabel: {},
             position: "right",
+            scale: true,
         }, ],
         series: [],
         useUTC: false,
     };
 
     #energyUseColors = {
         "Air temperature": "#0880A4",
@@ -114,118 +115,79 @@
         });
     }
 
     #showTSInfo(tsInfoCallback = null) {
         tsInfoCallback?.();
     }
 
-    #optionToContent(opt, dataset, timeFormat) {
-        let timestamps = opt.series[0].data.map((serieData) => {
-            return echarts.time.format(serieData[0], timeFormat);
-        });
-
+    #optionToContent(opt, timeFormat) {
         let mainContainerElmt = document.createElement("div");
         mainContainerElmt.classList.add("m-2", "me-3");
 
-        let subtitleElmt = document.createElement("h5");
-        subtitleElmt.innerText = opt.title[0].subtext;
-        mainContainerElmt.appendChild(subtitleElmt);
-
-        let tableContainerElmt = document.createElement("div");
-        tableContainerElmt.classList.add("table-responsive");
-
-        let tableElmt = document.createElement("table");
-        tableElmt.classList.add("table", "table-sm", "table-hover", "table-bordered", "caption-top", "user-select-all");
-        let tableCaptionElmt = document.createElement("caption");
-        tableCaptionElmt.classList.add("fst-italic", "text-muted", "text-end");
-        tableCaptionElmt.innerText = `${timestamps.length.toString()} rows`;
-        tableElmt.appendChild(tableCaptionElmt);
-        let tableHeadElmt = document.createElement("thead");
-        let tableHeadTrElmt = document.createElement("tr");
-        tableHeadTrElmt.classList.add("align-middle");
-        let tableHeadTimestampElmt = document.createElement("th");
-        tableHeadTimestampElmt.setAttribute("scope", "col");
-        tableHeadTimestampElmt.innerText = "Timestamp";
-        tableHeadTrElmt.appendChild(tableHeadTimestampElmt);
-        for (let serie of opt.series) {
-            let tableHeadThElmt = document.createElement("th");
-            tableHeadThElmt.setAttribute("scope", "col");
-            tableHeadThElmt.innerText = serie.name + (serie.unit ? ` (${serie.unit})` : "");
-            tableHeadTrElmt.appendChild(tableHeadThElmt);
-        }
-        tableHeadElmt.appendChild(tableHeadTrElmt);
-        tableElmt.appendChild(tableHeadElmt);
-        let tableBodyElmt = document.createElement("tbody");
-        tableBodyElmt.classList.add("table-group-divider");
-        for (let [index, timestamp] of timestamps.entries()) {
-            let tableTrElmt = document.createElement("tr");
-            let tableCellTimestampElmt = document.createElement("td");
-            tableCellTimestampElmt.innerText = timestamp;
-            tableTrElmt.appendChild(tableCellTimestampElmt);
+        if (opt.series.length > 0) {
+            let timestamps = opt.series[0].data.map((serieData) => {
+                return echarts.time.format(serieData[0], timeFormat);
+            });
+
+            let subtitleElmt = document.createElement("h5");
+            subtitleElmt.innerText = opt.title[0].subtext;
+            mainContainerElmt.appendChild(subtitleElmt);
+
+            let tableContainerElmt = document.createElement("div");
+            tableContainerElmt.classList.add("table-responsive");
+
+            let tableElmt = document.createElement("table");
+            tableElmt.classList.add("table", "table-sm", "table-hover", "table-bordered", "caption-top", "user-select-all");
+            let tableCaptionElmt = document.createElement("caption");
+            tableCaptionElmt.classList.add("fst-italic", "text-muted", "text-end");
+            tableCaptionElmt.innerText = `${timestamps.length.toString()} rows`;
+            tableElmt.appendChild(tableCaptionElmt);
+            let tableHeadElmt = document.createElement("thead");
+            let tableHeadTrElmt = document.createElement("tr");
+            tableHeadTrElmt.classList.add("align-middle");
+            let tableHeadTimestampElmt = document.createElement("th");
+            tableHeadTimestampElmt.setAttribute("scope", "col");
+            tableHeadTimestampElmt.innerText = "Timestamp";
+            tableHeadTrElmt.appendChild(tableHeadTimestampElmt);
             for (let serie of opt.series) {
-                if (serie.data && serie.data[index]) {
-                    let tableCellElmt = document.createElement("td");
-                    tableCellElmt.innerText = serie.data[index][1].toString();
-                    tableTrElmt.appendChild(tableCellElmt);
-                }
+                let tableHeadThElmt = document.createElement("th");
+                tableHeadThElmt.setAttribute("scope", "col");
+                tableHeadThElmt.innerText = serie.name;
+                tableHeadTrElmt.appendChild(tableHeadThElmt);
             }
-            tableBodyElmt.appendChild(tableTrElmt);
-        }
-        tableElmt.appendChild(tableBodyElmt);
-
-        tableContainerElmt.appendChild(tableElmt);
-        mainContainerElmt.appendChild(tableContainerElmt);
-        return mainContainerElmt;
-    }
-
-    #tooltipFormatter(params, dataset, timeFormat) {
-        let tooltipContainerElmt = document.createElement("div");
-
-        let ulElmt = document.createElement("ul");
-        ulElmt.classList.add("list-unstyled", "mx-2", "mt-2", "mb-0");
-
-        for (let [index, serieParams] of params.entries()) {
-            if (index == 0) {
-                let timeElmt = document.createElement("h6");
-                timeElmt.innerText = echarts.time.format(serieParams.value[0], timeFormat);
-                tooltipContainerElmt.appendChild(timeElmt);
-            }
-
-            let liElmt = document.createElement("li");
-            liElmt.classList.add("d-flex", "justify-content-between", "gap-4");
-            ulElmt.appendChild(liElmt);
-
-            let serieNameElmt = document.createElement("div");
-            serieNameElmt.classList.add("d-flex", "align-items-center", "gap-1");
-            serieNameElmt.innerHTML = `${serieParams.marker}<span>${serieParams.seriesName}</span>`;
-
-            let serieValueContainerElmt = document.createElement("div");
-            serieValueContainerElmt.classList.add("d-flex", "gap-1");
-
-            let serieValueElmt = document.createElement("span");
-            serieValueElmt.classList.add("fw-bold");
-            serieValueElmt.innerText = Parser.parseFloatOrDefault(serieParams.value[1], Number.NaN, 2).toString();
-            serieValueContainerElmt.appendChild(serieValueElmt);
-
-            let serieValueUnitElmt = document.createElement("small");
-            for (let [key, value] of Object.entries(dataset)) {
-                for (let [key2, value2] of Object.entries(value)) {
-                    if (value2.name == serieParams.seriesName) {
-                        serieValueUnitElmt.innerText = value2.timeseries.unit_symbol;
+            tableHeadElmt.appendChild(tableHeadTrElmt);
+            tableElmt.appendChild(tableHeadElmt);
+            let tableBodyElmt = document.createElement("tbody");
+            tableBodyElmt.classList.add("table-group-divider");
+            for (let [index, timestamp] of timestamps.entries()) {
+                let tableTrElmt = document.createElement("tr");
+                let tableCellTimestampElmt = document.createElement("td");
+                tableCellTimestampElmt.innerText = timestamp;
+                tableTrElmt.appendChild(tableCellTimestampElmt);
+                for (let serie of opt.series) {
+                    if (serie.data && serie.data[index]) {
+                        let tableCellElmt = document.createElement("td");
+                        tableCellElmt.innerText = serie.data[index][1].toString();
+                        tableTrElmt.appendChild(tableCellElmt);
                     }
                 }
+                tableBodyElmt.appendChild(tableTrElmt);
             }
-            serieValueContainerElmt.appendChild(serieValueUnitElmt);
+            tableElmt.appendChild(tableBodyElmt);
 
-            liElmt.appendChild(serieNameElmt);
-            liElmt.appendChild(serieValueContainerElmt);
+            tableContainerElmt.appendChild(tableElmt);
+            mainContainerElmt.appendChild(tableContainerElmt);
+        } else {
+            let noDataElmt = document.createElement("p");
+            noDataElmt.classList.add("fst-italic", "text-center", "text-muted");
+            noDataElmt.innerText = "No data";
+            mainContainerElmt.appendChild(noDataElmt);
         }
 
-        tooltipContainerElmt.appendChild(ulElmt);
-        return tooltipContainerElmt;
+        return mainContainerElmt;
     }
 
     connectedCallback() {
         this.#chart = echarts.init(this, this.#theme, this.#initOptions);
         this.#chart.setOption(this.#defaultOptions);
 
         this.#initEventListeners();
@@ -247,95 +209,77 @@
         this.#chart.hideLoading();
     }
 
     load(name, dataset, timeFormat, tsInfoCallback = null) {
         this.hideLoading();
 
         let options = this.#chart.getOption();
-        let listUnit = {
-            0: [],
-            1: []
-        };
 
         options.legend[0].data = [];
         options.legend[1].data = [];
 
-        options.title[0].text = `${name}`;
+        options.title[0].text = name;
 
         options.toolbox[0].feature.dataView.optionToContent = (opt) => {
-            return this.#optionToContent(opt, dataset, timeFormat);
+            return this.#optionToContent(opt, timeFormat);
         };
-
+        options.toolbox[0].feature.myTSInfo.show = tsInfoCallback != null;
         options.toolbox[0].feature.myTSInfo.onclick = () => {
             this.#showTSInfo(tsInfoCallback);
         };
 
-        options.tooltip[0].formatter = (params) => {
-            return this.#tooltipFormatter(params, dataset, timeFormat);
-        };
-
         options.series.length = 0;
 
+        let listUnit = {
+            0: [],
+            1: []
+        };
         let series = [];
         for (let [_parameter, serieParams] of Object.entries(dataset)) {
             for (let [_settings, value] of Object.entries(serieParams)) {
-                let chartData = Object.entries(value.data).map(([date, value]) => [date, Parser.parseFloatOrDefault(value, Number.NaN, 2)]);
-                if (chartData.length > 0) {
+                if (Object.values(value.data).length > 0) {
                     let serie = {
-                        name: value.name,
+                        name: `${value.name}${value.timeseries.unit_symbol != null ? ` [${value.timeseries.unit_symbol}]` : ""}`,
                         type: "line",
-                        data: Object.entries(value.data).map(([date, value]) => [date, Parser.parseFloatOrDefault(value, Number.NaN, 2)]),
+                        data: Object.entries(value.data).map(([date, value]) => {
+                            return [date, Parser.parseFloatOrDefault(value, Number.NaN, 2)];
+                        }),
                         emphasis: {
-                            focus: "series"
+                            focus: "series",
                         },
                         itemStyle: {
-                            color: this.#energyUseColors[value.name]
+                            color: this.#energyUseColors[value.name],
                         },
                         lineStyle: {
-                            width: 2,
                             type: value.name.includes("forecast") ? "dashed" : "solid",
                         },
                         yAxisIndex: value.yAxis,
-                        unit: value.timeseries.unit_symbol,
+                        symbol: "path://",
+                        connectNulls: true,
                     };
                     series.push(serie);
-                    if (!listUnit[value.yAxis].includes(serie.unit))
-                        listUnit[value.yAxis].push(serie.unit);
 
-                    options.legend[value.yAxis].data.push(value.name);
+                    if (value.timeseries.unit_symbol != null && !listUnit[value.yAxis].includes(value.timeseries.unit_symbol)) {
+                        listUnit[value.yAxis].push(value.timeseries.unit_symbol);
+                    }
+
+                    options.legend[value.yAxis].data.push(serie.name);
                 }
             }
         }
         options.series = series;
 
-        options.yAxis[0].data = options.series.map((serie) => serie.name);
-        options.yAxis[0].axisLabel.formatter = (value, index) => {
-            return `${value} (${listUnit[0]})`;
-        };
-
-        options.yAxis[1].data = options.series.map((serie) => serie.name);
-        options.yAxis[1].axisLabel.formatter = (value, index) => {
-            return `${value} (${listUnit[1]})`;
-        };
+        options.yAxis[0].name = listUnit[0].join(", ");
+        options.yAxis[1].name = listUnit[1].join(", ");
 
         if (options.legend[1].data.length == 0) {
             options.legend[0].left = "center";
             options.legend[0].width = "auto";
         };
 
-        options.legend[0].formatter = (name) => {
-            let serie = options.series.find((serie) => serie.name == name);
-            return `${name} (${serie.unit})`;
-        };
-
-        options.legend[1].formatter = (name) => {
-            let serie = options.series.find((serie) => serie.name == name);
-            return `${name} (${serie.unit})`;
-        };
-
         // Fix for bug, see: https://github.com/apache/incubator-echarts/issues/6202
         this.#chart.clear();
 
         this.#chart.setOption(options);
     }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/dropZone.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/dropZone.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/eventLevel.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/eventLevel.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/filterSelect.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/filterSelect.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/flash.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/flash.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/itemsCount.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/itemsCount.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     Parser
-} from "../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 import {
     Spinner
-} from "./spinner.js";
+} from "/static/scripts/modules/components/spinner.js";
 
 
 export class ItemsCount extends HTMLElement {
 
     #totalCount = 0;
     #firstItem = 0;
     #lastItem = 0;
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/modalConfirm.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/pagination.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/pagination.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/spinner.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/spinner.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -35,27 +35,44 @@
         super();
 
         this.#initOptions = options;
         this.#tzTool = new TimezoneTool();
 
         this.#loadOptions(options);
         this.#cacheDOM();
+
+        this.#dateInputElmt = document.createElement("input");
+        this.#dateInputElmt.type = "date";
+        this.#timeInputElmt = document.createElement("input");
+        this.#timeInputElmt.type = "time";
     }
 
     static get observedAttributes() {
         return ["disabled", "required"];
     }
 
     get date() {
         return this.#date;
     }
+    set date(value) {
+        this.#date = value;
+        this.#dateInputElmt.value = this.#date;
+        this.#updateDateInputFormBind();
+        this.#updateStyle();
+    }
 
     get time() {
         return this.#time;
     }
+    set time(value) {
+        this.#time = value;
+        this.#timeInputElmt.value = this.#time;
+        this.#updateTimeInputFormBind();
+        this.#updateStyle();
+    }
 
     get dateMin() {
         return this.#dateMin;
     }
     set dateMin(value) {
         this.#dateMin = value;
         this.#updateDateBounds();
@@ -80,16 +97,16 @@
     get hasDatetime() {
         return this.#dateInputElmt.value != "" && this.#dateInputElmt.value != null;
     }
 
     #loadOptions(options = {}) {
         this.#dateInputFormBind = this.getAttribute("date-input-form-bind") || options.dateInputFormBind;
         this.#timeInputFormBind = this.getAttribute("time-input-form-bind") || options.timeInputFormBind;
-        this.#isRequired = options?.required == null ? this.hasAttribute("required") : options.required;
-        this.#hasAutofocus = options?.autofocus == null ? this.hasAttribute("autofocus") : options.autofocus;
+        this.#isRequired = options?.required == null ? this.hasAttribute("required") : Parser.parseBoolOrDefault(options.required, false);
+        this.#hasAutofocus = options?.autofocus == null ? this.hasAttribute("autofocus") : Parser.parseBoolOrDefault(options.autofocus, false);
         this.#title = this.getAttribute("title") || options.title;
         this.#tzName = this.getAttribute("tzname") || options.tzName || this.#tzTool.defaultTzName;
         this.#dateMin = this.getAttribute("min") || options.dateMin;
         this.#dateMax = this.getAttribute("max") || options.dateMax;
         this.#date = this.getAttribute("date") || options.date;
         this.#time = this.getAttribute("time") || options.time;
         this.#usedAsFilter = this.getAttribute("as-filter") || Parser.parseBoolOrDefault(options.usedAsFilter, false);
@@ -243,32 +260,28 @@
         if (this.#title != null) {
             this.#titleSpanElmt = document.createElement("span");
             this.#titleSpanElmt.classList.add("input-group-text");
             this.#titleSpanElmt.innerText = this.#title;
             this.appendChild(this.#titleSpanElmt);
         }
 
-        this.#dateInputElmt = document.createElement("input");
         this.#dateInputElmt.classList.add("form-control");
-        this.#dateInputElmt.type = "date";
         if (this.#hasAutofocus) {
             this.#dateInputElmt.setAttribute("autofocus", true);
         }
         if (this.#dateMin != null) {
             this.#dateInputElmt.setAttribute("min", this.#dateMin);
         }
         if (this.#dateMax != null) {
             this.#dateInputElmt.setAttribute("max", this.#dateMax);
         }
         this.#dateInputElmt.style.minWidth = "125px";
         this.appendChild(this.#dateInputElmt);
 
-        this.#timeInputElmt = document.createElement("input");
         this.#timeInputElmt.classList.add("form-control");
-        this.#timeInputElmt.type = "time";
         this.#timeInputElmt.style.minWidth = "75px";
         this.appendChild(this.#timeInputElmt);
 
         if (this.#isRequired) {
             this.setRequired();
         } else {
             this.setOptional();
@@ -287,20 +300,26 @@
 
         this.#initEventListeners();
     }
 
     attributeChangedCallback(name, oldValue, newValue) {
         if (oldValue != newValue) {
             if (name == "disabled") {
+                if (newValue == null || newValue == "") {
+                    newValue = true;
+                }
                 if (newValue) {
                     this.setDisabled();
                 } else {
                     this.setEnabled();
                 }
             } else if (name == "required") {
+                if (newValue == null || newValue == "") {
+                    newValue = true;
+                }
                 if (newValue) {
                     this.setRequired();
                 } else {
                     this.setOptional();
                 }
             }
         }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/tzPicker.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/selector.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -238,14 +238,16 @@
     #internalAPIRequester = null;
     #filterReqIDs = {};
     #searchReqID = null;
     #selectReqID = null;
     #sitesTreeReqID = null;
     #zonesTreeReqID = null;
 
+    #searchNameTimeoutID = null;
+
     #messagesElmt = null;
 
     #selectedItemsContainerElmt = null;
     #clearSelectionBtnElmt = null;
     #selectedItems = [];
     #dropdownSearchPanelElmt = null;
     #bsDropdownSearchPanel = null;
@@ -346,16 +348,23 @@
             this.clearAllSelection();
         });
 
         this.#searchInputElmt.addEventListener("input", (event) => {
             event.preventDefault();
 
             this.#updateSearchInput();
-            this.#searchResultsPaginationElmt.page = 1;
-            this.refresh();
+
+            if (this.#searchNameTimeoutID != null) {
+                window.clearTimeout(this.#searchNameTimeoutID);
+                this.#searchNameTimeoutID = null;
+            }
+            this.#searchNameTimeoutID = window.setTimeout(() => {
+                this.#searchResultsPaginationElmt.page = 1;
+                this.refresh();
+            }, 700);
         });
 
         this.#filtersRemoveBtnElmt.addEventListener("click", (event) => {
             event.preventDefault();
 
             let hasFilterChanged = false;
             if (this.#searchInputElmt.value != "") {
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/tree.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/tree.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -53,38 +53,40 @@
         this.#treeContainerElmt = document.createElement("div");
         this.#treeContainerElmt.classList.add("nav-tree");
 
         this.#toolbarElmt = document.createElement("div");
         this.#toolbarElmt.classList.add("d-flex", "flex-nowrap", "align-items-start", "gap-3", "ms-auto");
 
         this.#collapseAllBtnElmt = document.createElement("a");
-        this.#collapseAllBtnElmt.classList.add("link-primary", "text-decoration-none", "text-nowrap");
+        this.#collapseAllBtnElmt.classList.add("link-primary", "text-decoration-none", "text-nowrap", "hstack", "align-items-center");
         this.#collapseAllBtnElmt.setAttribute("role", "button");
+        this.#collapseAllBtnElmt.title = "Collapse all nodes";
         this.#toolbarElmt.appendChild(this.#collapseAllBtnElmt);
 
         let collapseIconElmt = document.createElement("i");
         collapseIconElmt.classList.add("bi", "bi-arrows-collapse", "me-1");
         this.#collapseAllBtnElmt.appendChild(collapseIconElmt);
 
         let collapseTextElmt = document.createElement("small");
-        collapseTextElmt.classList.add("text-nowrap");
+        collapseTextElmt.classList.add("text-nowrap", "d-none", "d-sm-inline");
         collapseTextElmt.innerText = "collapse all";
         this.#collapseAllBtnElmt.appendChild(collapseTextElmt);
 
         this.#expandAllBtnElmt = document.createElement("a");
-        this.#expandAllBtnElmt.classList.add("link-primary", "text-decoration-none", "text-nowrap");
+        this.#expandAllBtnElmt.classList.add("link-primary", "text-decoration-none", "text-nowrap", "hstack", "align-items-center");
         this.#expandAllBtnElmt.setAttribute("role", "button");
+        this.#expandAllBtnElmt.title = "Expand all nodes";
         this.#toolbarElmt.appendChild(this.#expandAllBtnElmt);
 
         let expandIconElmt = document.createElement("i");
         expandIconElmt.classList.add("bi", "bi-arrows-expand", "me-1");
         this.#expandAllBtnElmt.appendChild(expandIconElmt);
 
         let expandTextElmt = document.createElement("small");
-        expandTextElmt.classList.add("text-nowrap");
+        expandTextElmt.classList.add("text-nowrap", "d-none", "d-sm-inline");
         expandTextElmt.innerText = "expand all";
         this.#expandAllBtnElmt.appendChild(expandTextElmt);
     }
 
     #initEventListeners() {
         this.#collapseAllBtnElmt?.addEventListener("click", () => {
             this.collapseAll();
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/flashTimer.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/flashTimer.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/formController.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/formController.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/notifications.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/sidebar.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/sidebar.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,44 +1,44 @@
 import {
     Parser
-} from "./tools/parser.js"
+} from "/static/scripts/modules/tools/parser.js"
 
 
 export class Sidebar {
 
     #navLinkElmts = null;
 
     #sidebarMenuInnerElmt = null;
-    #campaignSelectorNavLinkElmt = null;
-    #campaignsNavLinkElmt = null;
+    #campaignSelectedNavLinkElmt = null;
 
     constructor() {
         this.#cacheDOM();
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#navLinkElmts = [].slice.call(document.querySelectorAll(".app-sidebar .nav-link"));
 
         this.#sidebarMenuInnerElmt = document.querySelector("#sidebarMenu div.position-sticky");
-        this.#campaignSelectorNavLinkElmt = document.getElementById("campaignSelectorNavLink");
-        this.#campaignsNavLinkElmt = document.getElementById("campaignsNavLink");
+        this.#campaignSelectedNavLinkElmt = document.querySelector("#sidebarMenu #campaignSelectedNavItem > a.nav-link");
     }
 
     #initEventListeners() {
         window.addEventListener("resize", () => {
-            this.#updateCampaignSelectorWidth();
+            this.#updateCampaignSelectedWidth();
         });
     }
 
-    #updateCampaignSelectorWidth() {
-        let campaignNavStyle = window.getComputedStyle(this.#campaignSelectorNavLinkElmt.parentElement);
-        let remainingWidth = this.#sidebarMenuInnerElmt.clientWidth - this.#campaignsNavLinkElmt.clientWidth - Parser.parseFloatOrDefault(campaignNavStyle.gap);
-        if (Parser.parseFloatOrDefault(this.#campaignSelectorNavLinkElmt.style.maxWidth) != remainingWidth) {
-            this.#campaignSelectorNavLinkElmt.style.maxWidth = `${remainingWidth}px`;
+    #updateCampaignSelectedWidth() {
+        if (this.#campaignSelectedNavLinkElmt != null) {
+            let campaignNavStyle = window.getComputedStyle(this.#campaignSelectedNavLinkElmt.parentElement);
+            let remainingWidth = this.#sidebarMenuInnerElmt.clientWidth - Parser.parseFloatOrDefault(campaignNavStyle.gap);
+            if (Parser.parseFloatOrDefault(this.#campaignSelectedNavLinkElmt.style.maxWidth) != remainingWidth) {
+                this.#campaignSelectedNavLinkElmt.style.maxWidth = `${remainingWidth}px`;
+            }
         }
     }
 
     #setActive(elmt) {
         elmt?.classList.add("active", "fw-bold");
         elmt?.setAttribute("aria-current", "page");
         this.#tryOpenCollapse(elmt);
@@ -66,35 +66,42 @@
                 toggle: false
             });
             bsCollapse.show();
         }
     }
 
     refresh() {
-        // Set active the nav link element that corresponds to the current page location.
+        // Set active the "nav-link" element that corresponds to the current page location.
         let currentUrl = window.location.pathname + window.location.search;
 
-        // First search in nav-links.
+        // First search in "nav-link" class elements.
         let elmt = document.querySelector(`.app-sidebar .nav-link[href="${currentUrl}"]:not(.disabled)`);
         if (elmt == null) {
-            // Then search in dropdwn items.
+            // Then search in dropdown items.
             elmt = document.querySelector(`div.dropdown ul.dropdown-menu a.dropdown-item[href="${currentUrl}"]:not(.disabled)`)
             if (elmt != null) {
                 let dropdownMenuId = elmt.parentElement.parentElement.getAttribute("aria-labelledby");
                 let dropdownMenuElmt = document.getElementById(dropdownMenuId);
                 this.#setActive(dropdownMenuElmt);
             }
         }
         if (elmt == null) {
-            // And finally just search the best match in nav-links.
+            // And finally just search the best match in nav-link elements.
+            let elmtLocation = "";
             for (let navLinkElmt of this.#navLinkElmts) {
-                if (window.location.pathname.startsWith(navLinkElmt.getAttribute("href")?.split("?")[0])) {
-                    elmt = navLinkElmt;
-                    break;
+                let navLinkLocation = navLinkElmt.getAttribute("href")?.split("?")[0];
+                if (window.location.pathname.startsWith(navLinkLocation)) {
+                    // nav-link element location matches
+                    // 1. if first found, save it
+                    // 2. else verify that it is better than any other previous element found
+                    if (elmt == null || (elmt != null && navLinkLocation.length > elmtLocation.length)) {
+                        elmt = navLinkElmt;
+                        elmtLocation = navLinkLocation;
+                    }
                 }
             }
         }
         this.#setActive(elmt);
 
-        this.#updateCampaignSelectorWidth();
+        this.#updateCampaignSelectedWidth();
     }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/array.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/array.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/fetcher.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/fetcher.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/flaskES6.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/parser.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/parser.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/uuid.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/uuid.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/weather.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/weather.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -13,39 +13,42 @@
     Spinner
 } from "/static/scripts/modules/components/spinner.js";
 import {
     TimeseriesChartWeather
 } from "/static/scripts/modules/components/charts/tsChartWeather.js";
 import "/static/scripts/modules/components/tree.js";
 import {
-    TimeCalendar
+    TimeCalendar,
+    TimeDisplay
 } from "/static/scripts/modules/tools/time.js";
 
+
 export class WeatherExploreView {
 
     #internalAPIRequester = null;
     #retrieveDataReqID = null;
     #sitesTreeReqID = null;
 
     #messagesElmt = null;
     #mainChartContainerElmt = null;
     #periodTypeSelectElmt = null;
     #periodDaySelectElmt = null;
     #periodMonthSelectElmt = null;
     #periodYearSelectElmt = null;
     #sitesTreeElmt = null;
 
-    #forecast = null;
-    #forecastWrapper = null;
+    #forecastSwitchElmt = null;
+    #forecastWrapperElmt = null;
 
     #tzName = "UTC";
     #yearRef = null;
     #monthRef = null;
     #dayRef = null;
     #maxPastYears = 20;
+    #forecastNbDays = 5;
 
     #structuralElementType = null;
     #structuralElementId = null;
     #chartWeather = {};
 
     #previousPeriodType = null;
     #previousDaySelected = null;
@@ -58,16 +61,17 @@
         "Year-Daily": "{dd} {MMMM} {yyyy}",
         "Last-Day": "{dd} {MMMM} {yyyy} {HH}:{mm}",
         "Last-Week": "{dd} {MMMM} {yyyy} {HH}:{mm}",
         "Last-Month": "{dd} {MMMM} {yyyy} {HH}:{mm}",
         "Last-Year": "{dd} {MMMM} {yyyy}",
     };
 
-    constructor(tzName = "UTC", year = null, month = null) {
+    constructor(tzName = "UTC", forecastNbDays = 5, year = null, month = null) {
         this.#tzName = tzName || "UTC";
+        this.#forecastNbDays = forecastNbDays;
 
         let date = new Date();
         this.#yearRef = year || date.getUTCFullYear();
         this.#monthRef = month || date.getUTCMonth() + 1;
         this.#dayRef = date.getDate();
 
         this.#cacheDOM();
@@ -83,27 +87,27 @@
         this.#mainChartContainerElmt = document.getElementById("chartContainer");
 
         this.#sitesTreeElmt = document.getElementById("sitesTree");
         this.#periodTypeSelectElmt = document.getElementById("periodType");
         this.#periodDaySelectElmt = document.getElementById("periodDay");
         this.#periodMonthSelectElmt = document.getElementById("periodMonth");
         this.#periodYearSelectElmt = document.getElementById("periodYear");
-        this.#forecast = document.getElementById("forecastSwitch");
-        this.#forecastWrapper = document.getElementById("forecastWrapper");
+        this.#forecastSwitchElmt = document.getElementById("forecastSwitch");
+        this.#forecastWrapperElmt = document.getElementById("forecastWrapper");
     }
 
     #initEventListeners() {
         this.#sitesTreeElmt.addEventListener("treeNodeSelect", (event) => {
             this.#structuralElementType = event.detail.type;
             this.#structuralElementId = event.detail.id;
 
             this.#generateCharts();
         });
 
-        this.#forecast.addEventListener("change", (event) => {
+        this.#forecastSwitchElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
             this.#generateCharts();
         });
 
         this.#periodTypeSelectElmt.addEventListener("change", (event) => {
             event.preventDefault();
@@ -118,70 +122,50 @@
             this.#previousDaySelected = this.#periodDaySelectElmt.value;
             this.#generateCharts();
         });
 
         this.#periodMonthSelectElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            this.#updateDaysInMonth();
+            this.#updateDaysInMonth(this.#periodYearSelectElmt.value, this.#periodMonthSelectElmt.value, this.#previousDaySelected);
             this.#previousDaySelected = this.#periodDaySelectElmt.value;
             this.#generateCharts();
         });
 
         this.#periodYearSelectElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            this.#updateDaysInMonth();
+            this.#updateDaysInMonth(this.#periodYearSelectElmt.value, this.#periodMonthSelectElmt.value, this.#previousDaySelected);
             this.#previousDaySelected = this.#periodDaySelectElmt.value;
             this.#previousYearSelected = this.#periodYearSelectElmt.value;
             this.#generateCharts();
         });
     }
 
-    #getMonthName(month) {
-        const date = new Date();
-        date.setMonth(month - 1);
-
-        return date.toLocaleString([], {
-            month: "long"
-        });
-    }
-
     #updatePeriodSelect() {
         if (this.#previousPeriodType == null) {
             this.#periodYearSelectElmt.innerHTML = "";
             for (let year = this.#yearRef; year >= this.#yearRef - this.#maxPastYears; year--) {
                 let option = document.createElement("option");
                 option.value = year;
                 option.textContent = year;
+                option.selected = year == this.#yearRef;
                 this.#periodYearSelectElmt.appendChild(option);
             }
 
             this.#periodMonthSelectElmt.innerHTML = "";
             for (let month = 1; month <= 12; month++) {
                 let option = document.createElement("option");
                 option.value = month;
-                option.textContent = this.#getMonthName(month);
-                if (month == this.#monthRef) {
-                    option.selected = true;
-                }
+                option.textContent = TimeDisplay.getMonthName(month);
+                option.selected = month == this.#monthRef;
                 this.#periodMonthSelectElmt.appendChild(option);
             }
 
-            this.#periodDaySelectElmt.innerHTML = "";
-            const daysInMonth = TimeCalendar.getDaysInMonth(this.#yearRef, this.#monthRef);
-            for (let day = 1; day <= new Date(this.#yearRef, daysInMonth, 0).getDate(); day++) {
-                let option = document.createElement("option");
-                option.value = day;
-                option.textContent = day;
-                if (day == this.#dayRef) {
-                    option.selected = true;
-                }
-                this.#periodDaySelectElmt.appendChild(option);
-            }
+            this.#updateDaysInMonth(this.#yearRef, this.#monthRef, this.#dayRef);
         }
 
         if (this.#periodTypeSelectElmt.value.startsWith("Month")) {
             if (this.#previousPeriodType == null) {
                 this.#periodMonthSelectElmt.value = this.#monthRef.toString();
             }
             this.#periodMonthSelectElmt.classList.remove("d-none", "invisible");
@@ -197,104 +181,116 @@
             this.#periodMonthSelectElmt.classList.remove("d-none", "invisible");
         } else {
             this.#periodDaySelectElmt.classList.add("d-none", "invisible");
         }
 
         if (this.#periodTypeSelectElmt.value.startsWith("Last")) {
             this.#periodYearSelectElmt.classList.add("d-none", "invisible");
-            this.#forecastWrapper.classList.remove("d-none", "invisible");
+            this.#forecastWrapperElmt.classList.remove("d-none", "invisible");
         } else {
             this.#periodYearSelectElmt.classList.remove("d-none", "invisible");
-            this.#forecastWrapper.classList.add("d-none", "invisible");
-            this.#forecast.checked = false;
+            this.#forecastWrapperElmt.classList.add("d-none", "invisible");
+            this.#forecastSwitchElmt.checked = false;
         }
 
         this.#previousPeriodType = this.#periodTypeSelectElmt.value;
         this.#previousDaySelected = this.#periodDaySelectElmt.value;
         this.#previousYearSelected = this.#periodYearSelectElmt.value;
     }
 
-    #updateDaysInMonth() {
-        const daysInMonth = TimeCalendar.getDaysInMonth(this.#periodYearSelectElmt.value, this.#periodMonthSelectElmt.value);
+    #updateDaysInMonth(year, month, dayToSelect) {
         this.#periodDaySelectElmt.innerHTML = "";
-
+        let daysInMonth = TimeCalendar.getDaysInMonth(year, month);
+        let dayToSelectAdjusted = Math.min(dayToSelect, daysInMonth);
         for (let day = 1; day <= daysInMonth; day++) {
             let option = document.createElement("option");
             option.value = day;
             option.textContent = day;
-            if (day == this.#previousDaySelected) {
-                option.selected = true;
-            }
+            option.selected = day == dayToSelectAdjusted;
             this.#periodDaySelectElmt.appendChild(option);
         }
     }
 
-    #updateTsInfoModal(dataset, forecast, is_admin) {
-        let tsInfoModal = new bootstrap.Modal(document.getElementById("tsInfoModal"));
-        tsInfoModal.show();
-
-        let types = ["current", "forecast"];
-
-        if (!forecast) {
-            if (document.getElementById('forecast-tab').classList.contains('active')) {
-                document.getElementById('current-tab').classList.add('active');
-                document.getElementById('current').classList.add('show', 'active');
-                document.getElementById('forecast-tab').classList.remove('active');
-                document.getElementById('forecast').classList.remove('show', 'active');
+    #updateTsInfoModal(chartName, dataset) {
+        let tsInfoModalChartNameElmt = document.getElementById("tsInfoModalChartName");
+        tsInfoModalChartNameElmt.textContent = chartName;
+
+        let weatherTypes = ["current", "forecast"];
+        for (let weatherType of weatherTypes) {
+            let tabElmt = document.getElementById(`${weatherType}-tab`);
+            let tabContentElmt = document.getElementById(`${weatherType}-tabcontent`);
+            tabContentElmt.innerHTML = "";
+
+            if (weatherType == "current") {
+                let bsTab = new bootstrap.Tab(tabElmt);
+                bsTab.show();
+            } else if (weatherType == "forecast") {
+                if (this.#forecastSwitchElmt.checked) {
+                    tabElmt.classList.remove("disabled");
+                } else {
+                    tabElmt.classList.add("disabled");
+                }
             }
-            document.getElementById('forecast-tab').classList.add('disabled');
-        } else {
-            document.getElementById('forecast-tab').classList.remove('disabled');
-        }
 
-        for (let type of types) {
-            let tabContent = document.getElementById(type);
-            tabContent.innerHTML = "";
-
-            for (let [_key, value] of Object.entries(dataset)) {
-                let tsName = document.createElement("h5");
-                tsName.classList.add("fw-bold", "mt-3");
-                tsName.textContent = value[type].name;
-                tabContent.appendChild(tsName);
-
-                let tsDescription = document.createElement("p");
-                tsDescription.classList.add("fw-small");
-                tsDescription.textContent = value[type].timeseries.description;
-                tabContent.appendChild(tsDescription);
+            let tabContentContainerElmt = document.createElement("div");
+            tabContentContainerElmt.classList.add("vstack", "gap-3");
+            tabContentElmt.appendChild(tabContentContainerElmt);
+
+            for (let weatherParam of Object.values(dataset)) {
+                let weatherParamData = weatherParam[weatherType];
+
+                let paramContainerElmt = document.createElement("div");
+                tabContentContainerElmt.appendChild(paramContainerElmt);
+
+                let paramName = document.createElement("h6");
+                paramName.classList.add("fw-bold");
+                paramName.textContent = weatherParamData.name;
+                paramContainerElmt.appendChild(paramName);
+
+                let tsDescription = document.createElement("small");
+                tsDescription.classList.add("text-muted");
+                tsDescription.textContent = weatherParamData.timeseries.description;
+                paramContainerElmt.appendChild(tsDescription);
 
                 let row = document.createElement("div");
                 row.classList.add("row");
+                paramContainerElmt.appendChild(row);
 
                 let col1 = document.createElement("div");
                 col1.classList.add("col");
-
-                let periodValue = document.createElement("span");
-                periodValue.classList.add("fw-normal");
-                periodValue.textContent = value[type].timeseries.name ? value[type].timeseries.name + " [" + value[type].timeseries.unit_symbol + "]" : "No link for this parameter";
-                col1.appendChild(periodValue);
                 row.appendChild(col1);
 
-                if (is_admin) {
+                let tsName = document.createElement("span");
+                if (weatherParamData.timeseries.id != null) {
+                    tsName.textContent = `${weatherParamData.timeseries.name}${weatherParamData.timeseries.unit_symbol != null ? ` [${weatherParamData.timeseries.unit_symbol}]` : ""}`;
+                } else {
+                    tsName.classList.add("fst-italic", "text-warning");
+                    tsName.textContent = "No timeseries linked to this parameter";
+                }
+                col1.appendChild(tsName);
+
+                if (signedUser.is_admin && weatherParamData.timeseries.id != null) {
                     let col2 = document.createElement("div");
-                    col2.classList.add("col");
+                    col2.classList.add("col", "hstack", "gap-2");
+                    row.appendChild(col2);
 
-                    let id = document.createElement("p");
-                    id.textContent = "ID: ";
+                    let id = document.createElement("span");
+                    id.textContent = "ID";
                     id.classList.add("fw-bold");
+                    col2.appendChild(id);
 
                     let idValue = document.createElement("span");
-                    idValue.classList.add("fw-normal");
-                    idValue.textContent = value[type].timeseries.id;
-                    id.appendChild(idValue);
-                    col2.appendChild(id);
-                    row.appendChild(col2);
+                    idValue.textContent = weatherParamData.timeseries.id;
+                    col2.appendChild(idValue);
                 }
-                tabContent.appendChild(row);
             }
         }
+
+        let tsInfoModal = new bootstrap.Modal("#tsInfoModal");
+        tsInfoModal.show();
     }
 
     #generateCharts() {
         if (this.#structuralElementType != null && this.#structuralElementId != null) {
             for (let chart of Object.values(this.#chartWeather)) {
                 chart.dispose();
             }
@@ -313,15 +309,15 @@
                     `api.analysis.weather.retrieve`, {
                         site_id: this.#structuralElementId,
                         period_type: this.#periodTypeSelectElmt.value,
                         period_day: this.#periodDaySelectElmt.value,
                         period_month: this.#periodMonthSelectElmt.value,
                         period_year: this.#periodYearSelectElmt.value,
                         timezone: this.#tzName,
-                        forecast: this.#forecast.checked,
+                        forecast: this.#forecastSwitchElmt.checked ? this.#forecastNbDays : 0,
                     }
                 ),
                 (data) => {
                     this.#mainChartContainerElmt.innerHTML = "";
                     if (data == null || data.length == 0) {
                         let colElmt = document.createElement("div");
                         colElmt.classList.add("col", "text-start", "text-muted");
@@ -343,30 +339,29 @@
                             colElmt.appendChild(pHelpNotAdminElmt);
                         }
 
                         this.#mainChartContainerElmt.appendChild(colElmt);
                     } else {
                         for (let [name, dataset] of Object.entries(data)) {
                             let weatherChart = new TimeseriesChartWeather();
-
                             this.#chartWeather[name] = weatherChart;
 
                             let chartContainerElmt = document.createElement("div");
                             chartContainerElmt.classList.add("border", "border-1", "rounded", "justify-content-center", "bg-white", "p-2");
                             chartContainerElmt.appendChild(weatherChart);
 
                             let colElmt = document.createElement("div");
                             colElmt.classList.add("col");
                             colElmt.appendChild(chartContainerElmt);
 
                             this.#mainChartContainerElmt.appendChild(colElmt);
 
                             weatherChart.showLoading();
                             weatherChart.load(name, dataset, this.#timeFormatPerPeriodType[this.#periodTypeSelectElmt.value], () => {
-                                this.#updateTsInfoModal(dataset, this.#forecast.checked, signedUser.is_admin)
+                                this.#updateTsInfoModal(name, dataset)
                             });
                         }
                     }
                 },
                 (error) => {
                     this.#mainChartContainerElmt.innerHTML = "";
 
@@ -406,16 +401,16 @@
                         type: FlashMessageTypes.WARNING,
                         text: "No site available in this campaign",
                         isDismissible: false,
                         isTimed: false
                     });
                     this.#messagesElmt.appendChild(flashMsgElmt);
 
-                    document.querySelector("#periodType").disabled = true;
-                    document.querySelector("#forecastSwitch").disabled = true;
+                    this.#periodTypeSelectElmt.setAttribute("disabled", true);
+                    this.#forecastSwitchElmt.setAttribute("disabled", true);
                 }
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
                     text: error,
                     isDismissible: true
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/edit.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/edit.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/list.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/list.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
 import {
     flaskES6
-} from "../../../app.js";
+} from "/static/scripts/app.js";
 import {
     InternalAPIRequest
-} from "../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 import {
     Spinner
-} from "../../components/spinner.js";
-import "../../components/itemsCount.js";
-import "../../components/pagination.js";
-import "../../components/time/datetimePicker.js";
+} from "/static/scripts/modules/components/spinner.js";
+import "/static/scripts/modules/components/itemsCount.js";
+import "/static/scripts/modules/components/pagination.js";
+import "/static/scripts/modules/components/time/datetimePicker.js";
 import {
     FilterSelect
-} from "../../components/filterSelect.js";
+} from "/static/scripts/modules/components/filterSelect.js";
 import {
     TimeDisplay
-} from "../../tools/time.js";
+} from "/static/scripts/modules/tools/time.js";
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 import {
     EventLevelBadge
-} from "../../components/eventLevel.js";
+} from "/static/scripts/modules/components/eventLevel.js";
 import {
     StructuralElementSelector
-} from "../../components/structuralElements/selector.js";
+} from "/static/scripts/modules/components/structuralElements/selector.js";
 
 
 export class EventListView {
 
     #structuralElementTypes = []
     #tzName = "UTC";
     #defaultFilters = {};
@@ -42,14 +42,16 @@
     #filterReqIDs = {};
     #searchReqID = null;
     #loadEventInfoTabReqIDs = {};
     #loadEventInfoTabReqPageIDs = {};
     #sitesTreeReqID = null;
     #zonesTreeReqID = null;
 
+    #delayedUpdateTimeoutID = null;
+
     #messagesElmt = null;
 
     #filtersContainerElmt = null;
     #sourceSearchFilterElmt = null;
     #timestampMinSearchFilterElmt = null;
     #timestampMaxSearchFilterElmt = null;
     #btnRemoveFiltersElmt = null;
@@ -263,32 +265,44 @@
     }
 
     #initEventListeners() {
         this.#timestampMinSearchFilterElmt.addEventListener("datetimeChange", (event) => {
             event.preventDefault();
 
             this.#timestampMaxSearchFilterElmt.dateMin = this.#timestampMinSearchFilterElmt.date;
-            this.#paginationElmt.page = 1;
-            this.refresh();
+
+            this.#cancelDelayedUpdate();
+            this.#delayedUpdateTimeoutID = window.setTimeout(() => {
+                this.#paginationElmt.page = 1;
+                this.refresh();
+            }, 1000);
         });
 
         this.#timestampMaxSearchFilterElmt.addEventListener("datetimeChange", (event) => {
             event.preventDefault();
 
             this.#timestampMinSearchFilterElmt.dateMax = this.#timestampMaxSearchFilterElmt.date;
-            this.#paginationElmt.page = 1;
-            this.refresh();
+
+            this.#cancelDelayedUpdate();
+            this.#delayedUpdateTimeoutID = window.setTimeout(() => {
+                this.#paginationElmt.page = 1;
+                this.refresh();
+            }, 1000);
         });
 
         this.#sourceSearchFilterElmt.addEventListener("input", (event) => {
             event.preventDefault();
 
             this.#updateSourceSearch();
-            this.#paginationElmt.page = 1;
-            this.refresh();
+
+            this.#cancelDelayedUpdate();
+            this.#delayedUpdateTimeoutID = window.setTimeout(() => {
+                this.#paginationElmt.page = 1;
+                this.refresh();
+            }, 700);
         });
 
         this.#btnRemoveFiltersElmt.addEventListener("click", (event) => {
             event.preventDefault();
 
             let hasFilterChanged = false;
             if (this.#timestampMinSearchFilterElmt.date != null || this.#timestampMinSearchFilterElmt.time != null && this.#timestampMaxSearchFilterElmt.date != null || this.#timestampMaxSearchFilterElmt.time != null) {
@@ -938,15 +952,24 @@
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
+    #cancelDelayedUpdate() {
+        if (this.#delayedUpdateTimeoutID != null) {
+            window.clearTimeout(this.#delayedUpdateTimeoutID);
+            this.#delayedUpdateTimeoutID = null;
+        }
+    }
+
     refresh(afterResfreshCallback = null) {
+        this.#cancelDelayedUpdate();
+
         if (this.#searchReqID != null) {
             this.#internalAPIRequester.abort(this.#searchReqID);
             this.#searchReqID = null;
         }
 
         this.#itemsCountElmt.setLoading();
         this.#eventsContainerElmt.innerHTML = "";
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/explore.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/setup.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,19 @@
 import {
     InternalAPIRequest
-} from "../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
-    flaskES6
-} from "../../../app.js";
+    flaskES6,
+    signedUser
+} from "/static/scripts/app.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../components/flash.js";
-import "../../components/itemsCount.js";
+} from "/static/scripts/modules/components/flash.js";
+import "/static/scripts/modules/components/itemsCount.js";
 
 
 class ServiceCleanuManageView {
 
     #internalAPIRequester = null;
     #tsUpdateStateReqID = null;
 
@@ -35,37 +36,42 @@
 
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
-        this.#stateOnRadioElmt = document.getElementById("svc_state_on");
-        this.#stateOffRadioElmt = document.getElementById("svc_state_off");
-        this.#cleanupIDInputElmt = document.getElementById("cleanup_id");
-        this.#campaignIDInputElmt = document.getElementById("campaign_id");
-        this.#etagInputElmt = document.getElementById("etag");
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt = document.getElementById("svc_state_on");
+            this.#stateOffRadioElmt = document.getElementById("svc_state_off");
+            this.#cleanupIDInputElmt = document.getElementById("cleanup_id");
+            this.#campaignIDInputElmt = document.getElementById("campaign_id");
+            this.#etagInputElmt = document.getElementById("etag");
+        }
 
         this.#formFiltersElmt = document.getElementById("formFiltersElmt");
         this.#sortInputElmt = document.getElementById("sort");
         this.#sortRadioElmts = [].slice.call(document.querySelectorAll(`input[type="radio"][id^="sort-"]`));
     }
 
     #initEventListeners() {
-        this.#stateOnRadioElmt.addEventListener("change", () => {
-            if (this.#stateOnRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt.addEventListener("change", () => {
+                if (this.#stateOnRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+
+            this.#stateOffRadioElmt.addEventListener("change", () => {
+                if (this.#stateOffRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+        }
 
-        this.#stateOffRadioElmt.addEventListener("change", () => {
-            if (this.#stateOffRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
         for (let sortRadioElmt of this.#sortRadioElmts) {
             sortRadioElmt.addEventListener("change", (event) => {
                 event.preventDefault();
                 let sortData = sortRadioElmt.id.split("-");
                 let newSortValue = `${sortData[2].toLowerCase() == "asc" ? "+" : "-"}${sortData[1].toLowerCase()}`;
                 if (this.#sortInputElmt.value != newSortValue) {
                     this.#sortInputElmt.value = newSortValue;
@@ -136,15 +142,20 @@
                         isDismissible: true
                     });
                     this.#messagesElmt.appendChild(flashMsgElmt);
                 },
             );
         }
     }
+
+    mount() {
+
+    }
 }
 
 
 document.addEventListener("DOMContentLoaded", () => {
 
     let svcCleanupManageView = new ServiceCleanuManageView();
+    svcCleanupManageView.mount();
 
 });
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/list.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 import {
     flaskES6
-} from "../../../../app.js";
+} from "/static/scripts/app.js";
 import {
     InternalAPIRequest
-} from "../../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 import {
     Spinner
-} from "../../../components/spinner.js";
-import "../../../components/itemsCount.js";
+} from "/static/scripts/modules/components/spinner.js";
+import "/static/scripts/modules/components/itemsCount.js";
 import {
     Parser
-} from "../../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 
 
-class CheckMissingDataServiceListView {
+class CheckOutlierDataServiceListView {
 
     #internalAPIRequester = null;
     #searchReqID = null;
 
     #messagesElmt = null;
 
     #campaignNameSearchElmt = null;
@@ -118,32 +118,32 @@
             selectFilterElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
         }
     }
 
     #createEntryElement(entryData) {
         let isSelected = Parser.parseBoolOrDefault(entryData["is_selected"], false);
 
-        let manageUrl = flaskES6.urlFor(`services.missing_data.campaign_state`, {
+        let manageUrl = flaskES6.urlFor(`services.outlier_data.campaign_state`, {
             id: entryData["campaign_id"]
         });
         if (isSelected) {
-            manageUrl = flaskES6.urlFor(`services.missing_data.campaign_context_state`);
+            manageUrl = flaskES6.urlFor(`services.outlier_data.campaign_context_state`);
         } else if (entryData["id"] != null) {
-            manageUrl = flaskES6.urlFor(`services.missing_data.service_state`, {
+            manageUrl = flaskES6.urlFor(`services.outlier_data.service_state`, {
                 id: entryData["id"]
             });
         }
 
         let entryElmt = document.createElement("a");
         entryElmt.classList.add("list-group-item", "list-group-item-action", "d-flex", "gap-3", "py-3");
         if (isSelected) {
             entryElmt.classList.add("app-campaign-selected");
         }
         entryElmt.href = manageUrl;
-        entryElmt.title = "Manage campaign check missing data service";
+        entryElmt.title = "Manage campaign check outlier data service";
         let entryIconElmt = document.createElement("i");
         entryIconElmt.classList.add("bi", "bi-puzzle");
         entryElmt.appendChild(entryIconElmt);
 
         let entryContainerElmt = document.createElement("div");
         entryContainerElmt.classList.add("d-sm-flex", "d-grid", "justify-content-between", "gap-2", "w-100");
         entryElmt.appendChild(entryContainerElmt);
@@ -222,15 +222,15 @@
 
         if (this.#searchReqID != null) {
             this.#internalAPIRequester.abort(this.#searchReqID);
             this.#searchReqID = null;
         }
 
         this.#searchReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.services.missing_data.retrieve_list`, searchOptions),
+            flaskES6.urlFor(`api.services.outlier_data.retrieve_list`, searchOptions),
             (data) => {
                 this.#serviceStatesContainerElmt.innerHTML = "";
                 if (data.data.length > 0) {
                     for (let row of data.data) {
                         this.#serviceStatesContainerElmt.appendChild(this.#createEntryElement(row));
                     }
                 } else {
@@ -256,11 +256,11 @@
         );
     }
 }
 
 
 document.addEventListener("DOMContentLoaded", () => {
 
-    let view = new CheckMissingDataServiceListView();
+    let view = new CheckOutlierDataServiceListView();
     view.refresh();
 
 });
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,18 @@
 import {
     InternalAPIRequest
-} from "../../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
-    flaskES6
-} from "../../../../app.js";
+    flaskES6,
+    signedUser
+} from "/static/scripts/app.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 
 
 class CheckMissingDataServiceManageView {
 
     #internalAPIRequester = null;
     #updateStateReqID = null;
 
@@ -30,33 +31,37 @@
 
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
-        this.#stateOnRadioElmt = document.getElementById("svc_state_on");
-        this.#stateOffRadioElmt = document.getElementById("svc_state_off");
-        this.#campaignServiceIDInputElmt = document.getElementById("campaign_service_id");
-        this.#campaignIDInputElmt = document.getElementById("campaign_id");
-        this.#etagInputElmt = document.getElementById("etag");
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt = document.getElementById("svc_state_on");
+            this.#stateOffRadioElmt = document.getElementById("svc_state_off");
+            this.#campaignServiceIDInputElmt = document.getElementById("campaign_service_id");
+            this.#campaignIDInputElmt = document.getElementById("campaign_id");
+            this.#etagInputElmt = document.getElementById("etag");
+        }
     }
 
     #initEventListeners() {
-        this.#stateOnRadioElmt.addEventListener("change", () => {
-            if (this.#stateOnRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
-
-        this.#stateOffRadioElmt.addEventListener("change", () => {
-            if (this.#stateOffRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt.addEventListener("change", () => {
+                if (this.#stateOnRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+
+            this.#stateOffRadioElmt.addEventListener("change", () => {
+                if (this.#stateOffRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+        }
     }
 
     #updateServiceState(isEnabled) {
         if (this.#updateStateReqID != null) {
             this.#internalAPIRequester.abort(this.#updateStateReqID);
             this.#updateStateReqID = null;
         }
@@ -116,15 +121,20 @@
                         isDismissible: true
                     });
                     this.#messagesElmt.appendChild(flashMsgElmt);
                 },
             );
         }
     }
+
+    mount() {
+
+    }
 }
 
 
 document.addEventListener("DOMContentLoaded", () => {
 
     let view = new CheckMissingDataServiceManageView();
+    view.mount();
 
 });
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 import {
     flaskES6
-} from "../../../../app.js";
+} from "/static/scripts/app.js";
 import {
     InternalAPIRequest
-} from "../../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 import {
     Spinner
-} from "../../../components/spinner.js";
-import "../../../components/itemsCount.js";
+} from "/static/scripts/modules/components/spinner.js";
+import "/static/scripts/modules/components/itemsCount.js";
 import {
     Parser
-} from "../../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 
 
-class CheckOutlierDataServiceListView {
+class CheckMissingDataServiceListView {
 
     #internalAPIRequester = null;
     #searchReqID = null;
 
     #messagesElmt = null;
 
     #campaignNameSearchElmt = null;
@@ -118,32 +118,32 @@
             selectFilterElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
         }
     }
 
     #createEntryElement(entryData) {
         let isSelected = Parser.parseBoolOrDefault(entryData["is_selected"], false);
 
-        let manageUrl = flaskES6.urlFor(`services.outlier_data.campaign_state`, {
+        let manageUrl = flaskES6.urlFor(`services.missing_data.campaign_state`, {
             id: entryData["campaign_id"]
         });
         if (isSelected) {
-            manageUrl = flaskES6.urlFor(`services.outlier_data.campaign_context_state`);
+            manageUrl = flaskES6.urlFor(`services.missing_data.campaign_context_state`);
         } else if (entryData["id"] != null) {
-            manageUrl = flaskES6.urlFor(`services.outlier_data.service_state`, {
+            manageUrl = flaskES6.urlFor(`services.missing_data.service_state`, {
                 id: entryData["id"]
             });
         }
 
         let entryElmt = document.createElement("a");
         entryElmt.classList.add("list-group-item", "list-group-item-action", "d-flex", "gap-3", "py-3");
         if (isSelected) {
             entryElmt.classList.add("app-campaign-selected");
         }
         entryElmt.href = manageUrl;
-        entryElmt.title = "Manage campaign check outlier data service";
+        entryElmt.title = "Manage campaign check missing data service";
         let entryIconElmt = document.createElement("i");
         entryIconElmt.classList.add("bi", "bi-puzzle");
         entryElmt.appendChild(entryIconElmt);
 
         let entryContainerElmt = document.createElement("div");
         entryContainerElmt.classList.add("d-sm-flex", "d-grid", "justify-content-between", "gap-2", "w-100");
         entryElmt.appendChild(entryContainerElmt);
@@ -222,15 +222,15 @@
 
         if (this.#searchReqID != null) {
             this.#internalAPIRequester.abort(this.#searchReqID);
             this.#searchReqID = null;
         }
 
         this.#searchReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.services.outlier_data.retrieve_list`, searchOptions),
+            flaskES6.urlFor(`api.services.missing_data.retrieve_list`, searchOptions),
             (data) => {
                 this.#serviceStatesContainerElmt.innerHTML = "";
                 if (data.data.length > 0) {
                     for (let row of data.data) {
                         this.#serviceStatesContainerElmt.appendChild(this.#createEntryElement(row));
                     }
                 } else {
@@ -256,11 +256,11 @@
         );
     }
 }
 
 
 document.addEventListener("DOMContentLoaded", () => {
 
-    let view = new CheckOutlierDataServiceListView();
+    let view = new CheckMissingDataServiceListView();
     view.refresh();
 
 });
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,18 @@
 import {
     InternalAPIRequest
-} from "../../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
-    flaskES6
-} from "../../../../app.js";
+    flaskES6,
+    signedUser
+} from "/static/scripts/app.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 
 
 class CheckOutlierDataServiceManageView {
 
     #internalAPIRequester = null;
     #updateStateReqID = null;
 
@@ -30,33 +31,37 @@
 
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
-        this.#stateOnRadioElmt = document.getElementById("svc_state_on");
-        this.#stateOffRadioElmt = document.getElementById("svc_state_off");
-        this.#campaignServiceIDInputElmt = document.getElementById("campaign_service_id");
-        this.#campaignIDInputElmt = document.getElementById("campaign_id");
-        this.#etagInputElmt = document.getElementById("etag");
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt = document.getElementById("svc_state_on");
+            this.#stateOffRadioElmt = document.getElementById("svc_state_off");
+            this.#campaignServiceIDInputElmt = document.getElementById("campaign_service_id");
+            this.#campaignIDInputElmt = document.getElementById("campaign_id");
+            this.#etagInputElmt = document.getElementById("etag");
+        }
     }
 
     #initEventListeners() {
-        this.#stateOnRadioElmt.addEventListener("change", () => {
-            if (this.#stateOnRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
-
-        this.#stateOffRadioElmt.addEventListener("change", () => {
-            if (this.#stateOffRadioElmt.checked) {
-                this.#updateServiceState(this.#stateOnRadioElmt.checked);
-            }
-        });
+        if (signedUser.is_admin) {
+            this.#stateOnRadioElmt.addEventListener("change", () => {
+                if (this.#stateOnRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+
+            this.#stateOffRadioElmt.addEventListener("change", () => {
+                if (this.#stateOffRadioElmt.checked) {
+                    this.#updateServiceState(this.#stateOnRadioElmt.checked);
+                }
+            });
+        }
     }
 
     #updateServiceState(isEnabled) {
         if (this.#updateStateReqID != null) {
             this.#internalAPIRequester.abort(this.#updateStateReqID);
             this.#updateStateReqID = null;
         }
@@ -116,15 +121,20 @@
                         isDismissible: true
                     });
                     this.#messagesElmt.appendChild(flashMsgElmt);
                 },
             );
         }
     }
+
+    mount() {
+
+    }
 }
 
 
 document.addEventListener("DOMContentLoaded", () => {
 
     let view = new CheckOutlierDataServiceManageView();
+    view.mount();
 
 });
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 } from "/static/scripts/app.js";
 import {
     FlashMessageTypes,
     FlashMessage
 } from "/static/scripts/modules/components/flash.js";
 import {
     Spinner
-} from "../../../components/spinner.js";
+} from "/static/scripts/modules/components/spinner.js";
 import {
     FilterSelect
 } from "/static/scripts/modules/components/filterSelect.js";
 import "/static/scripts/modules/components/itemsCount.js";
 import "/static/scripts/modules/components/time/datetimePicker.js";
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,456 +1,331 @@
 import {
     InternalAPIRequest
-} from "../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     flaskES6,
     signedUser
-} from "../../../app.js";
+} from "/static/scripts/app.js";
 import {
     Spinner
-} from "../../components/spinner.js";
-import "../../components/itemsCount.js";
-import "../../components/pagination.js";
+} from "/static/scripts/modules/components/spinner.js";
 import {
-    FlashMessageTypes,
-    FlashMessage
-} from "../../components/flash.js";
+    Parser
+} from "/static/scripts/modules/tools/parser.js";
 import {
     TimeDisplay
-} from "../../tools/time.js";
+} from "/static/scripts/modules/tools/time.js";
 import {
     EventLevelBadge
-} from "../../components/eventLevel.js";
-import "../../components/tree.js";
-
+} from "/static/scripts/modules/components/eventLevel.js";
+import "/static/scripts/modules/components/itemsCount.js";
+import "/static/scripts/modules/components/pagination.js";
+import {
+    FlashMessageTypes,
+    FlashMessage
+} from "/static/scripts/modules/components/flash.js";
+import {
+    StructuralElementSelector
+} from "/static/scripts/modules/components/structuralElements/selector.js";
 
-export class StructuralElementsExploreView {
 
-    #tzName = "UTC";
-    #messagesElmt = null;
+export class TimeseriesListView {
 
     #internalAPIRequester = null;
-    #generalReqID = null;
-    #propertiesReqID = null;
-    #tsReqID = null;
-    #eventsReqID = null;
+    #getStructElmtsReqID = null;
+    #getPropDataReqID = null;
+    #getStatsReqID = {};
+    #getEventsReqID = null;
     #sitesTreeReqID = null;
     #zonesTreeReqID = null;
 
-    #tabSitesElmts = null;
-    #tabPropertiesElmts = null;
-    #generalTabContentElmt = null;
-    #propertiesTabContentElmt = null;
-
-    #tsSearchElmt = null;
-    #tsClearSearchBtnElmt = null;
-    #tsRecurseSwitchElmt = null;
-    #tsPageSizeElmt = null;
-    #tsCountElmt = null;
-    #tsPaginationElmt = null;
-    #tsListElmt = null;
-
-    #eventsSearchElmt = null;
-    #eventsClearSearchBtnElmt = null;
-    #eventsRecurseSwitchElmt = null;
-    #eventsPageSizeElmt = null;
-    #eventsCountElmt = null;
-    #eventsPaginationElmt = null;
-    #eventsListElmt = null;
-
-    #tabSitesSelected = null;
-    #tabPropertiesSelected = null;
-
-    #selectedItemsPerTab = {};
-    #renderPerTab = {
-        "general-tab": this.#renderGeneral.bind(this),
-        "properties-tab": this.#renderProperties.bind(this),
-        "timeseries-tab": this.#renderTimeseries.bind(this),
-        "events-tab": this.#renderEvents.bind(this),
-    }
-    #alreadyLoadedPerTab = {};
+    #tzName = "UTC";
 
-    #sitesTreeElmt = null;
-    #zonesTreeElmt = null;
+    #messagesElmt = null;
+    #formFiltersElmt = null;
+    #campaignScopeElmt = null;
+    #pageInputElmt = null;
+    #pageSizeElmt = null;
+    #pageLinkElmts = null;
+    #accordionTimeseriesBtnElmts = null;
+
+    #siteSelector = null;
+    #zoneSelector = null;
+    #structuralElementIdInputElmt = null;
+    #structuralElementRecursiveSwitchElmt = null;
+    #zoneIdInputElmt = null;
 
     constructor(options = {}) {
         this.#internalAPIRequester = new InternalAPIRequest();
 
         this.#loadOptions(options);
         this.#cacheDOM();
         this.#initEventListeners();
-
-        this.#updateTsSearchState();
-        this.#updateEventsSearchState();
     }
 
     #loadOptions(options = {}) {
+        this.filters = options.filters || {};
         this.#tzName = options.timezone || "UTC";
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
+        this.#formFiltersElmt = document.getElementById("formFilters");
+        this.#campaignScopeElmt = document.getElementById("campaign_scope");
+        this.#pageInputElmt = document.getElementById("page");
+        this.#pageSizeElmt = document.getElementById("page_size");
+        this.#pageLinkElmts = [].slice.call(document.querySelectorAll(".page-item:not(.disabled) .page-link"));
+        this.#accordionTimeseriesBtnElmts = [].slice.call(document.querySelectorAll("#accordionTimeseries .accordion-collapse.collapse"));
+
+        this.#structuralElementIdInputElmt = document.getElementById("structural_element_filter");
+        this.#structuralElementRecursiveSwitchElmt = document.getElementById("structural_element_recursive");
+        this.#zoneIdInputElmt = document.getElementById("zone_filter");
 
-        this.#tabSitesElmts = [].slice.call(document.querySelectorAll("#tabSites button[data-bs-toggle='tab']"));
-        this.#tabPropertiesElmts = [].slice.call(document.querySelectorAll("#tabProperties button[data-bs-toggle='tab']"));
-        this.#generalTabContentElmt = document.getElementById("general-tabcontent");
-        this.#propertiesTabContentElmt = document.getElementById("properties-tabcontent");
-
-        this.#tsSearchElmt = document.getElementById("tsSearch");
-        this.#tsClearSearchBtnElmt = document.getElementById("tsClear");
-        this.#tsRecurseSwitchElmt = document.getElementById("tsRecurseSwitch");
-        this.#tsPageSizeElmt = document.getElementById("tsPageSize");
-        this.#tsCountElmt = document.getElementById("tsCount");
-        this.#tsPaginationElmt = document.getElementById("tsPagination");
-        this.#tsListElmt = document.getElementById("tsList");
-
-        this.#eventsSearchElmt = document.getElementById("eventsSearch");
-        this.#eventsClearSearchBtnElmt = document.getElementById("eventsClear");
-        this.#eventsRecurseSwitchElmt = document.getElementById("eventsRecurseSwitch");
-        this.#eventsPageSizeElmt = document.getElementById("eventsPageSize");
-        this.#eventsCountElmt = document.getElementById("eventsCount");
-        this.#eventsPaginationElmt = document.getElementById("eventsPagination");
-        this.#eventsListElmt = document.getElementById("eventsList");
-
-        this.#sitesTreeElmt = document.getElementById("sitesTree");
-        this.#zonesTreeElmt = document.getElementById("zonesTree");
+        this.#siteSelector = StructuralElementSelector.getInstance("siteSelector");
+        this.#zoneSelector = StructuralElementSelector.getInstance("zoneSelector");
     }
 
     #initEventListeners() {
-        for (let tabElmt of this.#tabSitesElmts) {
-            if (tabElmt.classList.contains("active")) {
-                this.#tabSitesSelected = tabElmt;
-            }
-            this.#selectedItemsPerTab[tabElmt.id] = null;
-            tabElmt.addEventListener("shown.bs.tab", (event) => {
-                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
-                this.#tabSitesSelected = event.target;
-                for (let tabPropertyElmt of this.#tabPropertiesElmts) {
-                    this.#alreadyLoadedPerTab[tabPropertyElmt.id] = false;
-                }
-                this.#refreshTabs();
-            });
-        }
-
-        for (let tabElmt of this.#tabPropertiesElmts) {
-            if (tabElmt.classList.contains("active")) {
-                this.#tabPropertiesSelected = tabElmt;
-            }
-            this.#alreadyLoadedPerTab[tabElmt.id] = false;
-            tabElmt.addEventListener("shown.bs.tab", (event) => {
-                // newly activated tab is `event.target` ; previous active tab is `event.relatedTarget`
-                this.#tabPropertiesSelected = event.target;
-                this.#refreshTabs();
-            });
-        }
-
-        this.#tsSearchElmt.addEventListener("input", (event) => {
+        this.#campaignScopeElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            this.#updateTsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#tsPaginationElmt.page = 1;
-            this.#refreshTabs();
+            if (event.target.options[event.target.selectedIndex].value != this.filters.campaign_scope_id) {
+                this.#pageInputElmt.value = 1;
+                event.target.classList.remove("border-info", "bg-info", "bg-opacity-10");
+            } else {
+                this.#pageInputElmt.value = this.filters.page;
+                event.target.classList.add("border-info", "bg-info", "bg-opacity-10");
+            }
         });
 
-        this.#tsClearSearchBtnElmt.addEventListener("click", (event) => {
+        this.#pageSizeElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            this.#tsSearchElmt.value = "";
-            this.#updateTsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+            this.#pageInputElmt.value = 1;
+            this.#formFiltersElmt.submit();
         });
 
-        this.#tsRecurseSwitchElmt.addEventListener("change", (event) => {
-            event.preventDefault();
+        for (let pageLinkElmt of this.#pageLinkElmts) {
+            pageLinkElmt.addEventListener("click", (event) => {
+                event.preventDefault();
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
-        });
+                this.#pageInputElmt.value = pageLinkElmt.getAttribute("data-page");
+                this.#formFiltersElmt.submit();
+            });
+        }
 
-        this.#tsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
-            event.preventDefault();
+        for (let accordionTimeseriesBtnElmt of this.#accordionTimeseriesBtnElmts) {
+            accordionTimeseriesBtnElmt.addEventListener("show.bs.collapse", (event) => {
+                let tsId = event.target.getAttribute("data-ts-id");
+                this.#renderProperties(tsId);
+                this.#renderStructuralElements(tsId);
+                this.#renderStats(tsId);
+                this.#renderEvents(tsId);
+            });
+        }
 
-            if (event.detail.newValue != event.detail.oldValue) {
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-                this.#tsPaginationElmt.page = 1;
-                this.#refreshTabs();
+        this.#siteSelector.addEventListener("treeNodeSelect", (event) => {
+            if (event.detail.type == "space") {
+                this.#structuralElementRecursiveSwitchElmt.checked = false;
+                this.#structuralElementRecursiveSwitchElmt.setAttribute("disabled", true);
+            } else {
+                this.#structuralElementRecursiveSwitchElmt.removeAttribute("disabled");
             }
-        });
-
-        this.#tsPaginationElmt.addEventListener("pageItemClick", (event) => {
-            event.preventDefault();
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+            this.#structuralElementIdInputElmt.name = `${this.#structuralElementRecursiveSwitchElmt.checked ? "recurse_" : ""}${event.detail.type}_id`;
+            this.#structuralElementIdInputElmt.value = event.detail.id;
         });
 
-        this.#eventsSearchElmt.addEventListener("input", (event) => {
-            event.preventDefault();
-
-            this.#updateEventsSearchState();
+        this.#siteSelector.addEventListener("treeNodeUnselect", () => {
+            this.#structuralElementRecursiveSwitchElmt.removeAttribute("disabled");
 
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#eventsPaginationElmt.page = 1;
-            this.#refreshTabs();
+            this.#structuralElementIdInputElmt.name = this.#structuralElementIdInputElmt.id;
+            this.#structuralElementIdInputElmt.value = "";
         });
 
-        this.#eventsClearSearchBtnElmt.addEventListener("click", (event) => {
-            event.preventDefault();
-
-            this.#eventsSearchElmt.value = "";
-            this.#updateEventsSearchState();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+        this.#zoneSelector.addEventListener("treeNodeSelect", (event) => {
+            this.#zoneIdInputElmt.value = event.detail.id;
         });
 
-        this.#eventsRecurseSwitchElmt.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
+        this.#zoneSelector.addEventListener("treeNodeUnselect", () => {
+            this.#zoneIdInputElmt.value = "";
         });
 
-        this.#eventsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
-            event.preventDefault();
-
-            if (event.detail.newValue != event.detail.oldValue) {
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-                this.#eventsPaginationElmt.page = 1;
-                this.#refreshTabs();
+        this.#structuralElementRecursiveSwitchElmt.addEventListener("change", (event) => {
+            if (this.#structuralElementIdInputElmt.value != "" && this.#structuralElementIdInputElmt.value != "space_id") {
+                if (event.target.checked) {
+                    this.#structuralElementIdInputElmt.name = `recurse_${this.#structuralElementIdInputElmt.name}`;
+                } else {
+                    this.#structuralElementIdInputElmt.name = this.#structuralElementIdInputElmt.name.replace("recurse_", "");
+                }
             }
         });
-
-        this.#eventsPaginationElmt.addEventListener("pageItemClick", (event) => {
-            event.preventDefault();
-
-            this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = false;
-            this.#refreshTabs();
-        });
-
-        this.#sitesTreeElmt.addEventListener("treeNodeSelect", (event) => {
-            this.render(event.detail.id, event.detail.type, event.detail.path);
-        });
-
-        this.#zonesTreeElmt.addEventListener("treeNodeSelect", (event) => {
-            this.render(event.detail.id, event.detail.type, event.detail.path);
-        });
-    }
-
-    #updateTsSearchState() {
-        if (this.#tsSearchElmt.value != "") {
-            this.#tsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
-            this.#tsClearSearchBtnElmt.classList.remove("d-none", "invisible");
-        } else {
-            this.#tsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
-            this.#tsClearSearchBtnElmt.classList.add("d-none", "invisible");
-        }
     }
 
-    #updateEventsSearchState() {
-        if (this.#eventsSearchElmt.value != "") {
-            this.#eventsSearchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
-            this.#eventsClearSearchBtnElmt.classList.remove("d-none", "invisible");
-        } else {
-            this.#eventsSearchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
-            this.#eventsClearSearchBtnElmt.classList.add("d-none", "invisible");
-        }
-    }
-
-    #getEditBtnHTML(type, id, tab = null) {
+    #getEditBtnHTML(id, tab = null) {
         if (signedUser.is_admin) {
             let editUrlParams = {
-                type: type,
                 id: id
             };
+            let editLabel = ``;
             if (tab != null) {
                 editUrlParams["tab"] = tab;
+                editLabel = ` ${tab}`;
             }
             try {
-                let editUrl = flaskES6.urlFor(`structural_elements.edit`, editUrlParams);
-                return `<a class="btn btn-sm btn-outline-primary text-nowrap" href="${editUrl}" role="button" title="Edit ${type}"><i class="bi bi-pencil"></i> Edit</a>`;
+                let editUrl = flaskES6.urlFor(`timeseries.edit`, editUrlParams);
+                return `<a class="btn btn-sm btn-outline-secondary ms-auto w-auto" href="${editUrl}" role="button" title="Edit${editLabel}"><i class="bi bi-pencil"></i> Edit${editLabel}</a>`;
             } catch (error) {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
+                console.error(error);
             }
         }
         return ``;
     }
 
-    #getGeneralHTML(data, path) {
-        let htmlContent = `<div class="d-flex justify-content-between align-items-start gap-3 mb-3">
-    <div>
-        <h5 class="text-break">${data.structural_element.name}</h5>
-        <h6 class="text-break">${path}</h6>
-    </div>
-    ${this.#getEditBtnHTML(data.type, data.structural_element.id)}
-</div>
-<p class="fst-italic text-muted text-break">${data.structural_element.description}</p>
-<div class="row">
-    <dl class="col">
-        <dt>IFC ID</dt>
-        <dd>${(data.structural_element.ifc_id != null && data.structural_element.ifc_id != "") ? data.structural_element.ifc_id : "-"}</dd>
-    </dl>
-</div>`;
-
-        if (data.type == "site") {
-            htmlContent += `<div class="row">
-    <dl class="col">
-        <dt>Latitude <small class="text-muted">[°]</small></dt>
-        <dd>${data.structural_element.latitude != null ? data.structural_element.latitude : "-"}</dd>
-    </dl>
-    <dl class="col">
-        <dt>Longitude <small class="text-muted">[°]</small></dt>
-        <dd>${data.structural_element.longitude != null ? data.structural_element.longitude : "-"}</dd>
-    </dl>
-</div>`;
-        }
-
-        return htmlContent;
-    }
-
-    #getItemHelpHTML(itemDescription, withSpace = true) {
+    #getPropertyHelpHTML(property) {
         let ret = ``;
-        if (itemDescription?.length > 0) {
+        if (property.description?.length > 0) {
             let abbrElmt = document.createElement("abbr");
-            abbrElmt.title = itemDescription != null ? itemDescription : "";
+            abbrElmt.title = property.description != null ? property.description : "";
             let abbrContentElmt = document.createElement("i");
             abbrContentElmt.classList.add("bi", "bi-question-diamond");
             abbrElmt.appendChild(abbrContentElmt);
-            ret = `<sup${withSpace ? ` class="ms-1"`: ``}>${abbrElmt.outerHTML}</sup>`;
+            ret = `<sup class="ms-1">${abbrElmt.outerHTML}</sup>`;
         }
         return ret;
     }
 
-    #getPropertiesHTML(data, id) {
+    #getPropertiesHTML(properties, tsId) {
         let propertyDataHTML = ``;
-        if (data.properties.length > 0) {
-            for (let property of data.properties) {
-                let unitSymbol = (property.unit_symbol != null && property.unit_symbol.length > 0) ? `<small class="text-muted ms-1">[${property.unit_symbol}]</small>` : ``;
+        if (properties.length > 0) {
+            for (let property of properties) {
+                let propVal = property.value;
+                switch (property.value_type) {
+                    case "integer":
+                        propVal = Parser.parseIntOrDefault(property.value, "-");
+                        break;
+                    case "float":
+                        propVal = Parser.parseFloatOrDefault(property.value, "-", 1);
+                        break;
+                    case "boolean":
+                        propVal = Parser.parseBoolOrDefault(property.value, "-");
+                        break;
+                }
+
+                let unitSymbol = (property.unit_symbol != null && property.unit_symbol.length > 0) ? `<span class="text-muted ms-1">[${property.unit_symbol}]</span>` : ``;
                 propertyDataHTML += `<dl>
-    <dt>${property.name}${unitSymbol}${this.#getItemHelpHTML(property.description)}</dt>
-    <dd>${(property.value !== "" && property.value != null) ? property.value : "-"}</dd>
+    <dt>${property.name}${unitSymbol}${this.#getPropertyHelpHTML(property)}</dt>
+    <dd>${propVal}</dd>
 </dl>`;
             }
         } else {
-            propertyDataHTML = `<p class="fst-italic">No data</p>`;
+            propertyDataHTML = `<p class="fst-italic">No attributes</p>`;
         }
 
         return `<div class="d-flex justify-content-between align-items-start mb-3">
     <div class="d-flex gap-4">
         ${propertyDataHTML}
     </div>
-    ${this.#getEditBtnHTML(data.type, id, "properties")}
-</div>`;
-    }
-
-    #getErrorHTML(error) {
-        return `<div class="alert alert-danger" role="alert">
-    <i class="bi bi-x-octagon me-2"></i>
-    ${error}
+    ${this.#getEditBtnHTML(tsId, "attributes")}
 </div>`;
     }
 
-    #renderGeneral(id, type, path) {
-        this.#generalTabContentElmt.innerHTML = "";
-        this.#generalTabContentElmt.appendChild(new Spinner());
-
-        if (this.#generalReqID != null) {
-            this.#internalAPIRequester.abort(this.#generalReqID);
-            this.#generalReqID = null;
-        }
-        this.#generalReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_data`, {
-                type: type,
-                id: id
-            }),
-            (data) => {
-                this.#generalTabContentElmt.innerHTML = this.#getGeneralHTML(data, path);
-            },
-            (error) => {
-                this.#generalTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
-            },
-        );
-    }
+    #getStructuralElementsHTML(data) {
+        let contentHTML = ``;
 
-    #renderProperties(id, type, path) {
-        this.#propertiesTabContentElmt.innerHTML = "";
-        this.#propertiesTabContentElmt.appendChild(new Spinner());
-
-        if (this.#propertiesReqID != null) {
-            this.#internalAPIRequester.abort(this.#propertiesReqID);
-            this.#propertiesReqID = null;
-        }
-        this.#propertiesReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.structural_elements.retrieve_property_data`, {
-                type: type,
-                id: id
-            }),
-            (data) => {
-                this.#propertiesTabContentElmt.innerHTML = this.#getPropertiesHTML(data, id);
-            },
-            (error) => {
-                this.#propertiesTabContentElmt.innerHTML = this.#getErrorHTML(error.message);
-            },
-        );
-    }
+        let totalLinks = 0;
+        for (let structuralElementType of data.structural_element_types) {
+            let structuralElementContentHTML = ``;
+            let nbLinks = 0;
+            for (let tsStructElmtLink of data.data[structuralElementType]) {
+                structuralElementContentHTML += `<div class="d-flex flex-nowrap align-items-center border rounded bg-white px-2 py-1 gap-1">
+<i class="bi bi-${structuralElementType == "zone" ? "bullseye" : "building"}"></i>
+<span class="fw-bold">${tsStructElmtLink[structuralElementType].name}</span>`;
+                if (structuralElementType != "zone" && tsStructElmtLink.path.length > 0) {
+                    structuralElementContentHTML += `<small class="text-muted ms-2">${tsStructElmtLink.path}</small>`;
+                }
+                structuralElementContentHTML += `</div>`;
 
-    #populateTimeseriesList(tsList) {
-        this.#tsListElmt.innerHTML = "";
-        if (tsList.length > 0) {
-            for (let tsData of tsList) {
-                let tsElmt = document.createElement("div");
-                tsElmt.classList.add("list-group-item");
+                totalLinks += 1;
+                nbLinks += 1;
+            }
 
-                let tsHeaderElmt = document.createElement("div");
-                tsHeaderElmt.classList.add("d-flex", "gap-1");
+            if (nbLinks > 0) {
+                contentHTML += `<div class="mb-3">
+    <h6 class="fw-bold text-capitalize">${structuralElementType}s (${nbLinks})</h6>
+    <div class="d-flex gap-2 mx-2">${structuralElementContentHTML}</div>
+</div>`;
+            }
+        }
 
-                let iconElmt = document.createElement("i");
-                iconElmt.classList.add("bi", "bi-clock-history", "me-1");
-                tsHeaderElmt.appendChild(iconElmt);
+        if (totalLinks <= 0) {
+            contentHTML = `<p class="fst-italic">No locations</p>`;
+        }
 
-                let nameSpanElmt = document.createElement("span");
-                nameSpanElmt.classList.add("fw-bold", "text-break");
-                nameSpanElmt.innerText = tsData.name;
-                tsHeaderElmt.appendChild(nameSpanElmt);
-
-                if (tsData.unit_symbol) {
-                    let unitSpanElmt = document.createElement("span");
-                    unitSpanElmt.classList.add("text-muted");
-                    unitSpanElmt.innerText = `[${tsData.unit_symbol}]`;
-                    tsHeaderElmt.appendChild(unitSpanElmt);
-                }
+        return `<div class="mb-3">
+    ${contentHTML}
+</div>`;
+    }
 
-                tsElmt.appendChild(tsHeaderElmt);
+    #populateStats(tsDataStats, statsContainerElmt) {
+        statsContainerElmt.innerHTML = "";
 
-                let tsDescElmt = document.createElement("small");
-                tsDescElmt.classList.add("fst-italic", "text-muted");
-                tsDescElmt.innerText = tsData.description != null ? tsData.description : "-";
-                tsElmt.appendChild(tsDescElmt);
+        let createListGroupItemElmt = (title, value) => {
+            let listGroupItemElmt = document.createElement("li");
+            listGroupItemElmt.classList.add("list-group-item", "d-flex", "align-items-center", "justify-content-between", "gap-2");
+            timestampsBoundsListElmt.appendChild(listGroupItemElmt);
+            let listGroupItemTitleElmt = document.createElement("h6");
+            listGroupItemTitleElmt.classList.add("fw-bold", "text-muted", "mb-0");
+            listGroupItemTitleElmt.innerText = title;
+            listGroupItemElmt.appendChild(listGroupItemTitleElmt);
+            let listGroupItemValueElmt = document.createElement("small");
+            listGroupItemValueElmt.classList.add("text-nowrap");
+            listGroupItemValueElmt.innerText = value;
+            listGroupItemElmt.appendChild(listGroupItemValueElmt);
+            return listGroupItemElmt;
+        };
 
-                this.#tsListElmt.appendChild(tsElmt);
-            }
-        } else {
-            let nodataSpanElmt = document.createElement("span");
-            nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
-            nodataSpanElmt.innerText = "No data";
-            this.#tsListElmt.appendChild(nodataSpanElmt);
-        }
+        let timestampsCardElmt = document.createElement("div");
+        timestampsCardElmt.classList.add("card", "mb-auto");
+        statsContainerElmt.appendChild(timestampsCardElmt);
+        let timestampsCardHeaderElmt = document.createElement("div");
+        timestampsCardHeaderElmt.classList.add("card-header", "fw-bold");
+        timestampsCardHeaderElmt.innerText = "Timestamps statistics";
+        timestampsCardElmt.appendChild(timestampsCardHeaderElmt);
+        let timestampsBoundsListElmt = document.createElement("ul");
+        timestampsBoundsListElmt.classList.add("list-group", "list-group-flush");
+        timestampsCardElmt.appendChild(timestampsBoundsListElmt);
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("First", tsDataStats["first_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["first_timestamp"]), {
+            timezone: this.#tzName
+        }) : "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Last", tsDataStats["last_timestamp"] != null ? TimeDisplay.toLocaleString(new Date(tsDataStats["last_timestamp"]), {
+            timezone: this.#tzName
+        }) : "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Period duration", tsDataStats["period_duration"] || "-"));
+        timestampsBoundsListElmt.appendChild(createListGroupItemElmt("Last data since", tsDataStats["last_data_since"] || "-"));
+
+        let statsCardElmt = document.createElement("div");
+        statsCardElmt.classList.add("card", "mb-auto");
+        statsContainerElmt.appendChild(statsCardElmt);
+        let statsCardHeaderElmt = document.createElement("div");
+        statsCardHeaderElmt.classList.add("card-header", "fw-bold");
+        statsCardHeaderElmt.innerText = "Values statistics";
+        statsCardElmt.appendChild(statsCardHeaderElmt);
+        let statsListElmt = document.createElement("ul");
+        statsListElmt.classList.add("list-group", "list-group-flush");
+        statsCardElmt.appendChild(statsListElmt);
+        statsListElmt.appendChild(createListGroupItemElmt("Count", Parser.parseIntOrDefault(tsDataStats["count"])));
+        statsListElmt.appendChild(createListGroupItemElmt("Minimum", Parser.parseFloatOrDefault(tsDataStats["min"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Maximum", Parser.parseFloatOrDefault(tsDataStats["max"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Average", Parser.parseFloatOrDefault(tsDataStats["avg"], Number.NaN, 2)));
+        statsListElmt.appendChild(createListGroupItemElmt("Standard deviation", Parser.parseFloatOrDefault(tsDataStats["stddev"], Number.NaN, 2)));
     }
 
-    #populateEventList(eventsList) {
-        this.#eventsListElmt.innerHTML = "";
+    #populateEventList(eventsList, eventsContainerElmt) {
+        eventsContainerElmt.innerHTML = "";
         if (eventsList.length > 0) {
             for (let eventData of eventsList) {
                 let eventElmt = document.createElement("div");
                 eventElmt.classList.add("list-group-item");
 
                 let eventHeaderElmt = document.createElement("div");
                 eventHeaderElmt.classList.add("d-flex", "align-items-center", "gap-1", "w-100");
@@ -477,251 +352,246 @@
 
                 let bodyContentElmt = document.createElement("div");
                 bodyContentElmt.classList.add("d-flex", "justify-content-between", "align-items-start", "gap-2");
                 eventElmt.appendChild(bodyContentElmt);
 
                 let eventDescElmt = document.createElement("small");
                 eventDescElmt.classList.add("fst-italic", "text-muted");
-                eventDescElmt.innerText = eventData.description;
+                eventDescElmt.innerText = eventData.description != null ? eventData.description : "-";
                 bodyContentElmt.appendChild(eventDescElmt);
 
                 let sourceElmt = document.createElement("span");
                 sourceElmt.classList.add("text-nowrap");
                 sourceElmt.innerText = eventData.source;
                 bodyContentElmt.appendChild(sourceElmt);
 
-                this.#eventsListElmt.appendChild(eventElmt);
+                eventsContainerElmt.appendChild(eventElmt);
             }
         } else {
             let nodataSpanElmt = document.createElement("span");
             nodataSpanElmt.classList.add("fst-italic", "text-muted", "text-center");
             nodataSpanElmt.innerText = "No data";
-            this.#eventsListElmt.appendChild(nodataSpanElmt);
+            eventsContainerElmt.appendChild(nodataSpanElmt);
         }
     }
 
-    #renderTimeseries(id, type, path) {
-        this.#tsCountElmt.setLoading();
-        this.#tsListElmt.innerHTML = "";
-        this.#tsListElmt.appendChild(new Spinner());
-
-        if (this.#tsReqID != null) {
-            this.#internalAPIRequester.abort(this.#tsReqID);
-            this.#tsReqID = null;
-        }
+    #getErrorHTML(error) {
+        return `<div class="alert alert-danger" role="alert">
+    <i class="bi bi-x-octagon me-2"></i>
+    ${error}
+</div>`;
+    }
 
-        if (["space", "zone"].includes(type)) {
-            this.#tsRecurseSwitchElmt.checked = false;
-            this.#tsRecurseSwitchElmt.setAttribute("disabled", true);
-        } else {
-            this.#tsRecurseSwitchElmt.removeAttribute("disabled");
+    #renderProperties(tsId) {
+        let timeseriesPropertiesElmt = document.getElementById(`timeseriesAttributes-${tsId}`);
+        let tsAlreadyLoaded = JSON.parse(timeseriesPropertiesElmt.getAttribute("data-ts-loaded"));
+        if (!tsAlreadyLoaded) {
+            timeseriesPropertiesElmt.innerHTML = "";
+            timeseriesPropertiesElmt.appendChild(new Spinner());
+
+            if (this.#getPropDataReqID != null) {
+                this.#internalAPIRequester.abort(this.#getPropDataReqID);
+                this.#getPropDataReqID = null;
+            }
+            this.#getPropDataReqID = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.timeseries.retrieve_property_data`, {
+                    id: tsId
+                }),
+                (data) => {
+                    timeseriesPropertiesElmt.innerHTML = this.#getPropertiesHTML(data, tsId);
+                    timeseriesPropertiesElmt.setAttribute("data-ts-loaded", true);
+                },
+                (error) => {
+                    timeseriesPropertiesElmt.innerHTML = this.#getErrorHTML(error.message);
+                },
+            );
         }
+    }
 
-        let tsOptions = {
-            "page_size": this.#tsPageSizeElmt.current,
-            "page": this.#tsPaginationElmt.page,
-        };
-        tsOptions[`${this.#tsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
-        if (this.#tsSearchElmt.value != "") {
-            tsOptions["search"] = this.#tsSearchElmt.value;
+    #renderStructuralElements(tsId) {
+        let timeseriesStructuralElementsElmt = document.getElementById(`timeseriesStructuralElements-${tsId}`);
+        let tsAlreadyLoaded = JSON.parse(timeseriesStructuralElementsElmt.getAttribute("data-ts-loaded"));
+        if (!tsAlreadyLoaded) {
+            timeseriesStructuralElementsElmt.innerHTML = "";
+            timeseriesStructuralElementsElmt.appendChild(new Spinner());
+
+            if (this.#getStructElmtsReqID != null) {
+                this.#internalAPIRequester.abort(this.#getStructElmtsReqID);
+                this.#getStructElmtsReqID = null;
+            }
+            this.#getStructElmtsReqID = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.timeseries.retrieve_structural_elements`, {
+                    id: tsId
+                }),
+                (data) => {
+                    timeseriesStructuralElementsElmt.innerHTML = this.#getStructuralElementsHTML(data);
+                    timeseriesStructuralElementsElmt.setAttribute("data-ts-loaded", true);
+                },
+                (error) => {
+                    timeseriesStructuralElementsElmt.innerHTML = this.#getErrorHTML(error.message);
+                },
+            );
         }
-
-        this.#tsReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.timeseries.retrieve_list`, tsOptions),
-            (data) => {
-                let tsPaginationOpts = {
-                    pageSize: this.#tsPageSizeElmt.current,
-                    totalItems: data.pagination.total,
-                    totalPages: data.pagination.total_pages,
-                    page: data.pagination.page,
-                    firstPage: data.pagination.first_page,
-                    lastPage: data.pagination.last_page,
-                    previousPage: data.pagination.previous_page,
-                    nextPage: data.pagination.next_page,
-                }
-                this.#tsPaginationElmt.reload(tsPaginationOpts);
-                this.#tsCountElmt.update({
-                    totalCount: this.#tsPaginationElmt.totalItems,
-                    firstItem: this.#tsPaginationElmt.startItem,
-                    lastItem: this.#tsPaginationElmt.endItem
-                });
-
-                this.#populateTimeseriesList(data.data);
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            },
-        );
     }
 
-    #renderEvents(id, type, path) {
-        this.#eventsCountElmt.setLoading();
-        this.#eventsListElmt.innerHTML = "";
-        this.#eventsListElmt.appendChild(new Spinner());
-
-        if (this.#eventsReqID != null) {
-            this.#internalAPIRequester.abort(this.#eventsReqID);
-            this.#eventsReqID = null;
+    #renderStats(tsId) {
+        let tsDataStatsStatesElmt = document.getElementById(`tsDataStatsStates-${tsId}`);
+        let tsDataStatsContainerElmt = document.getElementById(`tsDataStats-${tsId}`);
+        let alreadyLoaded = JSON.parse(tsDataStatsContainerElmt.getAttribute("data-ts-loaded"));
+
+        if (!alreadyLoaded) {
+            tsDataStatsContainerElmt.innerHTML = "";
+            tsDataStatsContainerElmt.appendChild(new Spinner());
+
+            if (this.#getStatsReqID[tsId] != null) {
+                this.#internalAPIRequester.abort(this.#getStatsReqID[tsId]);
+                this.#getStatsReqID[tsId] = null;
+            }
+            this.#getStatsReqID[tsId] = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.timeseries.data.retrieve_stats`, {
+                    data_state: tsDataStatsStatesElmt.value,
+                    timeseries: [tsId]
+                }),
+                (data) => {
+                    this.#populateStats(data[tsId.toString()], tsDataStatsContainerElmt);
+                    tsDataStatsContainerElmt.setAttribute("data-ts-loaded", true);
+                },
+                (error) => {
+                    tsDataStatsContainerElmt.innerHTML = this.#getErrorHTML(error);
+                },
+            );
+
+            tsDataStatsStatesElmt.addEventListener("change", () => {
+                tsDataStatsContainerElmt.setAttribute("data-ts-loaded", false);
+                this.#renderStats(tsId);
+            });
         }
+    }
 
-        if (["space", "zone"].includes(type)) {
-            this.#eventsRecurseSwitchElmt.checked = false;
-            this.#eventsRecurseSwitchElmt.setAttribute("disabled", true);
-        } else {
-            this.#eventsRecurseSwitchElmt.removeAttribute("disabled");
-        }
+    #renderEvents(tsId) {
+        let tsEventsPageSizeElmt = document.getElementById(`tsEventsPageSize-${tsId}`);
+        let tsEventsItemsCountElmt = document.getElementById(`tsEventsItemsCount-${tsId}`);
+        let tsEventsPaginationElmt = document.getElementById(`tsEventsPagination-${tsId}`);
+        let tsEventsContainerElmt = document.getElementById(`tsEvents-${tsId}`);
+        let alreadyLoaded = JSON.parse(tsEventsContainerElmt.getAttribute("data-ts-loaded"));
+
+        if (!alreadyLoaded) {
+            tsEventsContainerElmt.innerHTML = "";
+            tsEventsContainerElmt.appendChild(new Spinner());
+
+            if (this.#getEventsReqID != null) {
+                this.#internalAPIRequester.abort(this.#getEventsReqID);
+                this.#getEventsReqID = null;
+            }
 
-        let eventsOptions = {
-            "page_size": this.#eventsPageSizeElmt.current,
-            "page": this.#eventsPaginationElmt.page,
-        };
-        eventsOptions[`${this.#eventsRecurseSwitchElmt.checked ? "recurse_" : ""}${type}_id`] = id;
-        if (this.#eventsSearchElmt.value != "") {
-            eventsOptions["in_source"] = this.#eventsSearchElmt.value;
-        }
+            tsEventsPageSizeElmt.addEventListener("pageSizeChange", (event) => {
+                event.preventDefault();
 
-        this.#eventsReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.events.retrieve_list`, eventsOptions),
-            (data) => {
-                let eventsPaginationOpts = {
-                    pageSize: this.#eventsPageSizeElmt.current,
-                    totalItems: data.pagination.total,
-                    totalPages: data.pagination.total_pages,
-                    page: data.pagination.page,
-                    firstPage: data.pagination.first_page,
-                    lastPage: data.pagination.last_page,
-                    previousPage: data.pagination.previous_page,
-                    nextPage: data.pagination.next_page,
+                if (event.detail.newValue != event.detail.oldValue) {
+                    tsEventsPaginationElmt.page = 1;
+                    tsEventsContainerElmt.setAttribute("data-ts-loaded", false);
+                    this.#renderEvents(tsId);
                 }
-                this.#eventsPaginationElmt.reload(eventsPaginationOpts);
-                this.#eventsCountElmt.update({
-                    totalCount: this.#eventsPaginationElmt.totalItems,
-                    firstItem: this.#eventsPaginationElmt.startItem,
-                    lastItem: this.#eventsPaginationElmt.endItem
-                });
+            });
+            tsEventsPaginationElmt.addEventListener("pageItemClick", (event) => {
+                event.preventDefault();
 
-                this.#populateEventList(data.data);
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error,
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            },
-        );
+                this.#renderEvents(tsId);
+            });
+
+            let eventsOptions = {
+                "page_size": tsEventsPageSizeElmt.current,
+                "page": tsEventsPaginationElmt.page,
+                "timeseries_id": tsId,
+            };
+            this.#getEventsReqID = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.events.retrieve_list`, eventsOptions),
+                (data) => {
+                    let eventsPaginationOpts = {
+                        pageSize: tsEventsPageSizeElmt.current,
+                        totalItems: data.pagination.total,
+                        totalPages: data.pagination.total_pages,
+                        page: data.pagination.page,
+                        firstPage: data.pagination.first_page,
+                        lastPage: data.pagination.last_page,
+                        previousPage: data.pagination.previous_page,
+                        nextPage: data.pagination.next_page,
+                    }
+                    tsEventsPaginationElmt.reload(eventsPaginationOpts);
+                    tsEventsItemsCountElmt.update({
+                        totalCount: tsEventsPaginationElmt.totalItems,
+                        firstItem: tsEventsPaginationElmt.startItem,
+                        lastItem: tsEventsPaginationElmt.endItem
+                    });
+
+                    this.#populateEventList(data.data, tsEventsContainerElmt);
+                    tsEventsContainerElmt.setAttribute("data-ts-loaded", true);
+                },
+                (error) => {
+                    tsEventsContainerElmt.innerHTML = this.#getErrorHTML(error.message);
+                },
+            );
+        }
     }
 
     #loadSitesTreeData() {
-        this.#sitesTreeElmt.showLoading();
+        this.#siteSelector.showLoadingTree();
 
         if (this.#sitesTreeReqID != null) {
             this.#internalAPIRequester.abort(this.#sitesTreeReqID);
             this.#sitesTreeReqID = null;
         }
 
         this.#sitesTreeReqID = this.#internalAPIRequester.get(
             flaskES6.urlFor(`api.structural_elements.retrieve_tree_sites`),
             (data) => {
-                this.#sitesTreeElmt.load(data.data);
-                this.#sitesTreeElmt.collapseAll();
+                this.#siteSelector.loadTree(data.data);
+
+                if (this.#structuralElementIdInputElmt.value != "") {
+                    let structuralElementType = this.#structuralElementIdInputElmt.name.replace("_id", "");
+                    this.#siteSelector.select(`${structuralElementType}-${this.#structuralElementIdInputElmt.value}`);
+                }
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
                     text: error,
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
     #loadZonesTreeData() {
-        this.#zonesTreeElmt.showLoading();
+        this.#zoneSelector.showLoadingTree();
 
         if (this.#zonesTreeReqID != null) {
             this.#internalAPIRequester.abort(this.#zonesTreeReqID);
             this.#zonesTreeReqID = null;
         }
 
         this.#zonesTreeReqID = this.#internalAPIRequester.get(
             flaskES6.urlFor(`api.structural_elements.retrieve_tree_zones`),
             (data) => {
-                this.#zonesTreeElmt.load(data.data);
-                this.#zonesTreeElmt.collapseAll();
+                this.#zoneSelector.loadTree(data.data);
+
+                if (this.#zoneIdInputElmt.value != "") {
+                    this.#zoneSelector.select(`zone-${this.#zoneIdInputElmt.value}`);
+                }
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
                     text: error,
                     isDismissible: true
                 });
                 this.#messagesElmt.appendChild(flashMsgElmt);
             },
         );
     }
 
-    #generateHelpElement(helpContext) {
-        let helpContainerElmt = document.createElement("div");
-        helpContainerElmt.classList.add("alert", "alert-info", "mb-0", "pb-0");
-
-        let helpIconElmt = document.createElement("i");
-        helpIconElmt.classList.add("bi", "bi-question-diamond", "me-2");
-        helpContainerElmt.appendChild(helpIconElmt);
-
-        let helpTitleElmt = document.createElement("span");
-        helpTitleElmt.classList.add("fw-bold");
-        helpTitleElmt.innerText = "Help";
-        helpContainerElmt.appendChild(helpTitleElmt);
-
-        let helpTextElmt = document.createElement("p");
-        helpTextElmt.innerHTML = `Select a <span class="fw-bold">location (site, building...)</span> in the tree to see its <span class="fw-bold">${helpContext}</span>.`;
-        helpContainerElmt.appendChild(helpTextElmt);
-
-        return helpContainerElmt;
-    }
-
-    #refreshTabs() {
-        let selectedItemData = this.#selectedItemsPerTab[this.#tabSitesSelected.id];
-        if (selectedItemData != null) {
-            if (!this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id]) {
-                this.#renderPerTab[this.#tabPropertiesSelected.id]?.call(this, selectedItemData.id, selectedItemData.type, selectedItemData.path);
-                this.#alreadyLoadedPerTab[this.#tabPropertiesSelected.id] = true;
-            }
-        } else {
-            this.#generalTabContentElmt.innerHTML = "";
-            this.#generalTabContentElmt.appendChild(this.#generateHelpElement("description"));
-            this.#propertiesTabContentElmt.innerHTML = "";
-            this.#propertiesTabContentElmt.appendChild(this.#generateHelpElement("properties"));
-            this.#tsListElmt.innerHTML = "";
-            this.#tsListElmt.appendChild(this.#generateHelpElement("related timeseries"));
-            this.#eventsListElmt.innerHTML = "";
-            this.#eventsListElmt.appendChild(this.#generateHelpElement("related events"));
-        }
-    }
-
-    render(id, type, path) {
-        this.#selectedItemsPerTab[this.#tabSitesSelected.id] = {
-            id: id,
-            type: type,
-            path: path
-        };
-        for (let tabElmt of this.#tabPropertiesElmts) {
-            this.#alreadyLoadedPerTab[tabElmt.id] = false;
-        }
-        this.#tsPaginationElmt.reload();
-        this.#refreshTabs();
-    }
-
-    refresh() {
+    mount() {
         this.#loadSitesTreeData();
         this.#loadZonesTreeData();
-        this.#refreshTabs();
     }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -143,14 +143,16 @@
 
 class TimeseriesDataExploreView {
 
     #internalAPIRequester = null;
     #tsDataStatesReqID = null;
     #tsDataGetReqID = null;
 
+    #updateChartTimeoutID = null;
+
     #messagesElmt = null;
 
     #chartContainerElmt = null;
     #chartExplore = null;
 
     #periodTypeElmt = null;
     #periodCustomElmt = null;
@@ -170,14 +172,16 @@
     #selectTimeseriesModalElmt = null;
     #selectTimeseriesModal = null;
     #tsSelector = null;
     #selectTimeseriesYAxisPositionContainerElmt = null;
     #selectTimeseriesSeriesTypeContainerElmt = null;
     #selectedTimeseriesSaveBtnElmt = null;
 
+    #defaultEndDate = null;
+    #defaultEndTime = null;
     #defaultTsDataState = "Clean";
     #defaultPeriodType = "last-24-hours";
     #defaultAggregationOperator = "avg";
     #defaultAggregationBucketWidth = {
         "unit": "hour",
         "value": 1,
     }
@@ -239,28 +243,39 @@
 
                 this.#periodStartDatetimeElmt.focus();
             } else {
                 this.#periodCustomElmt.classList.add("d-none", "invisible");
                 this.#periodStartDatetimeElmt.removeAttribute("required");
                 this.#periodEndDatetimeElmt.removeAttribute("required");
 
+                this.#periodEndDatetimeElmt.date = this.#defaultEndDate;
+                this.#periodEndDatetimeElmt.time = this.#defaultEndTime;
+
                 if (this.#periodTypeElmt.value != this.#periodTypeLoaded) {
                     this.#loadChartSeries();
                 }
             }
         });
 
-        this.#periodStartDatetimeElmt.addEventListener("dateChange", () => {
+        this.#periodStartDatetimeElmt.addEventListener("datetimeChange", () => {
             this.#periodEndDatetimeElmt.dateMin = this.#periodStartDatetimeElmt.date;
-            this.#loadChartSeries();
+
+            this.#cancelUpdateChart();
+            this.#updateChartTimeoutID = window.setTimeout(() => {
+                this.#loadChartSeries();
+            }, 1000);
         });
 
-        this.#periodEndDatetimeElmt.addEventListener("dateChange", () => {
+        this.#periodEndDatetimeElmt.addEventListener("datetimeChange", () => {
             this.#periodStartDatetimeElmt.dateMax = this.#periodEndDatetimeElmt.date;
-            this.#loadChartSeries();
+
+            this.#cancelUpdateChart();
+            this.#updateChartTimeoutID = window.setTimeout(() => {
+                this.#loadChartSeries();
+            }, 1000);
         });
 
         this.#aggInputElmt.addEventListener("change", () => {
             this.#updateAggregationBucketState();
             this.#loadChartSeries();
         });
 
@@ -705,15 +720,20 @@
 
                 aggregation = this.#aggInputElmt.value;
             }
 
             this.#tsDataGetReqID = this.#internalAPIRequester.get(
                 flaskES6.urlFor(`api.timeseries.data.retrieve_multiple_data_json`, urlParams),
                 (data) => {
-                    for (let [tsID, tsData] of Object.entries(data)) {
+                    // Iterate over each requested timeseries ID (instead of data from internal API response).
+                    // The main reason is that, in some cases (and especially with no aggregation requested), data can be empty and therefore chart series are not updated.
+                    for (let tsID of tsIDs) {
+                        // Get timeseries data or empty structure if not in data from internal API response.
+                        let tsData = data[tsID.toString()] || {};
+                        // Update timeseries chart series.
                         this.#chartExplore.updateSeriesData(tsID, tsData, {
                             aggregation: aggregation
                         });
                     }
                     this.#periodTypeLoaded = this.#periodTypeElmt.value;
 
                     this.#chartExplore.hideLoading();
@@ -743,15 +763,25 @@
         } else {
             // TODO: update all?
         }
 
         this.#chartExplore.hideLoading();
     }
 
+    #cancelUpdateChart() {
+        if (this.#updateChartTimeoutID != null) {
+            window.clearTimeout(this.#updateChartTimeoutID);
+            this.#updateChartTimeoutID = null;
+        }
+    }
+
     mount() {
+        this.#defaultEndDate = this.#periodEndDatetimeElmt.date;
+        this.#defaultEndTime = this.#periodEndDatetimeElmt.time;
+
         this.#loadDataStates();
 
         this.#chartExplore = new TimeseriesChartExplore({
             height: 600,
             width: "auto"
         });
         this.#chartContainerElmt.innerHTML = "";
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/delete.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
-import "../../components/itemsCount.js";
+import "/static/scripts/modules/components/itemsCount.js";
 import {
     Pagination,
     PageSizeSelector
-} from "../../components/pagination.js";
+} from "/static/scripts/modules/components/pagination.js";
 import {
     AccordionList
-} from "../../components/accordionList.js";
+} from "/static/scripts/modules/components/accordionList.js";
 import {
     DropZone
-} from "../../components/dropZone.js";
+} from "/static/scripts/modules/components/dropZone.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../components/flash.js";
+} from "/static/scripts/modules/components/flash.js";
 import {
     Spinner
-} from "../../components/spinner.js";
+} from "/static/scripts/modules/components/spinner.js";
 import {
     ModalConfirm
-} from "../../components/modalConfirm.js";
+} from "/static/scripts/modules/components/modalConfirm.js";
 import {
     InternalAPIRequest
-} from "../../tools/fetcher.js";
+} from "/static/scripts/modules/tools/fetcher.js";
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 import {
     flaskES6
-} from "../../../app.js";
-import "../../components/tree.js";
+} from "/static/scripts/app.js";
+import "/static/scripts/modules/components/tree.js";
 
 
 export class TimeseriesManageStructuralElementsView {
 
     #internalAPIRequester = null;
     #getTSListReqID = null;
     #sitesTreeReqID = null;
@@ -64,14 +64,15 @@
         this.#tsPageSizeSelectorContainerElmt.innerHTML = "";
         this.#tsPageSizeSelectorContainerElmt.appendChild(this.#tsPageSizeSelectorElmt);
 
         this.#tsListElmt = new AccordionList();
         this.#tsListContainerElmt.innerHTML = "";
         this.#tsListContainerElmt.appendChild(this.#tsListElmt);
 
+        this.#enableOrRefreshTooltips();
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
         this.#searchElmt = document.getElementById("search");
         this.#clearSearchBtnElmt = document.getElementById("clear");
@@ -102,35 +103,31 @@
             event.preventDefault();
 
             this.#update({
                 "page": event.detail.page
             });
         });
 
-        this.#searchElmt.addEventListener("input", (event) => {
+        // "input" event is fired each time the input text is updated (key pressed...)
+        // "change" event is only fired when losing focus or hitting enter key
+        this.#searchElmt.addEventListener("change", (event) => {
             event.preventDefault();
 
-            if (event.target.value != "") {
-                this.#clearSearchBtnElmt.classList.remove("d-none", "invisible");
-            } else {
-                this.#clearSearchBtnElmt.classList.add("d-none", "invisible");
-            }
-
+            this.#updateSearchState();
             this.#update({
                 "page_size": this.#tsPageSizeSelectorElmt.value,
                 "search": event.target.value
             });
         });
 
         this.#clearSearchBtnElmt.addEventListener("click", (event) => {
             event.preventDefault();
 
             this.#searchElmt.value = "";
-            this.#clearSearchBtnElmt.classList.add("d-none", "invisible");
-
+            this.#updateSearchState();
             this.#update({
                 "page_size": this.#tsPageSizeSelectorElmt.value
             });
         });
 
         this.#tsListElmt.addEventListener("accordionItemOpen", (event) => {
             event.preventDefault();
@@ -302,14 +299,32 @@
                         this.#messagesElmt.appendChild(flashMsgElmt);
                     },
                 );
             }
         });
     }
 
+    #enableOrRefreshTooltips() {
+        // Enable (or refresh) Bootstrap tooltips.
+        var tooltipTriggerList = [].slice.call(document.querySelectorAll(`[data-bs-toggle="tooltip"]`));
+        tooltipTriggerList.map((tooltipTriggerEl) => {
+            return new bootstrap.Tooltip(tooltipTriggerEl);
+        });
+    }
+
+    #updateSearchState() {
+        if (this.#searchElmt.value != "") {
+            this.#searchElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
+            this.#clearSearchBtnElmt.classList.remove("d-none", "invisible");
+        } else {
+            this.#searchElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
+            this.#clearSearchBtnElmt.classList.add("d-none", "invisible");
+        }
+    }
+
     #createDropedItemElement(id, icon, title, text, removeCallback) {
         let dropedItemElmt = document.createElement("div");
         dropedItemElmt.id = id;
         dropedItemElmt.classList.add("btn-group", "btn-group-sm", "rounded", "bg-white");
         dropedItemElmt.style.maxWidth = "350px";
 
         let dropItemMainContainerElmt = document.createElement("div");
@@ -488,8 +503,14 @@
     }
 
     refresh(options = {}) {
         this.#loadSitesTreeData();
         this.#loadZonesTreeData();
         this.#update(options);
     }
+
+    mount() {
+        this.#searchElmt.value = "";
+        this.#updateSearchState();
+        this.refresh();
+    }
 }
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/list.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/manageGroups.js` & `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/styles/signin.css` & `bemserver-ui-0.6.0/bemserver_ui/static/styles/signin.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/static/styles/tree.css` & `bemserver-ui-0.6.0/bemserver_ui/static/styles/tree.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/header.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/header.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 {% import "macros/components/sidebar.html" as mac_sidebar with context %}
-{% include "components/campaigns/selector.html" +%}
 <nav id="sidebarMenu" class="col-md-3 col-xl-2 d-md-block bg-light app-sidebar border-end border-2 collapse pb-4">
     <div class="position-sticky">
         <div class="d-flex flex-column gap-3">
             {% filter indent(width=12, first=True) %}
             {% include "components/sidebar/sidebar_campaign_selector.html" +%}
             {% include "components/sidebar/sidebar_campaign_context.html" %}
             {% set sidebar_plugins = get_sidebar_plugins(g.campaign_ctxt) %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_admin.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html`

 * *Files 20% similar despite different names*

```diff
@@ -10,16 +10,15 @@
                 </button>
             </h2>
             <div id="panelCollapseAdminSites" class="accordion-collapse collapse" aria-labelledby="panelHeadingAdminSites">
                 <div class="accordion-body px-0 py-2">
                     <ul class="nav nav-pills flex-column gap-1">
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
-                            {{- mac_sidebar.render_nav_link("Properties", url_for("structural_elements.properties.list"), "Manage locations properties", ["bi", "bi-card-list"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("structural_elements.properties.create"), "Add a new locations property", ["bi", "bi-plus-circle"]) -}}
+                            {{- mac_sidebar.render_nav_link("Attributes", url_for("structural_elements.properties.list"), "Manage sites attributes", ["bi", "bi-card-list"], extra_classes=["w-100"]) -}}
                             {% endfilter %}
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
         <div class="accordion-item border-0">
@@ -29,22 +28,20 @@
                 </button>
             </h2>
             <div id="panelCollapseAdminTS" class="accordion-collapse collapse" aria-labelledby="panelHeadingAdminTS">
                 <div class="accordion-body px-0 py-2">
                     <ul class="nav nav-pills flex-column gap-1">
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
-                            {{- mac_sidebar.render_nav_link("Properties", url_for("timeseries.properties.list"), "Manage timeseries properties", ["bi", "bi-card-list"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("timeseries.properties.create"), "Add a new timeseries property", ["bi", "bi-plus-circle"]) -}}
+                            {{- mac_sidebar.render_nav_link("Attributes", url_for("timeseries.properties.list"), "Manage timeseries attributes", ["bi", "bi-card-list"], extra_classes=["w-100"]) -}}
                             {% endfilter %}
                         </li>
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
-                            {{- mac_sidebar.render_nav_link("Data states", url_for("timeseries.datastates.list"), "Manage timeseries data states", ["bi", "bi-inboxes"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("timeseries.datastates.create"), "Add a new timeseries data state", ["bi", "bi-plus-circle"]) -}}
+                            {{- mac_sidebar.render_nav_link("Data states", url_for("timeseries.datastates.list"), "Manage timeseries data states", ["bi", "bi-tags"], extra_classes=["w-100"]) -}}
                             {% endfilter %}
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
         {% if g.campaign_ctxt.has_campaign %}
@@ -72,15 +69,15 @@
                     <span class="app-sidebar-heading"><i class="bi bi-puzzle"></i> Services</span>
                 </button>
             </h2>
             <div id="panelCollapseAdminServices" class="accordion-collapse collapse" aria-labelledby="panelHeadingAdminServices">
                 <div class="accordion-body px-0 py-2">
                     <ul class="nav nav-pills flex-column gap-1">
                         {% filter indent(width=24, first=True) %}
-                        {{- mac_sidebar.render_nav_item("Cleanup", url_for("services.cleanup.list"), "Manage cleanup service", ["bi", "bi-magic"]) -}}
+                        {{- mac_sidebar.render_nav_item("Cleanup data", url_for("services.cleanup.list"), "Manage cleanup data service", ["bi", "bi-magic"]) -}}
                         {{- mac_sidebar.render_nav_item("Check missing data", url_for("services.missing_data.list"), "Manage missing data service", ["bi", "bi-journal-x"]) -}}
                         {{- mac_sidebar.render_nav_item("Check outlier data", url_for("services.outlier_data.list"), "Manage check outlier data service", ["bi", "bi-layout-wtf"]) -}}
                         {% endfilter %}
                     </ul>
                 </div>
             </div>
         </div>
@@ -92,15 +89,14 @@
             </h2>
             <div id="panelCollapseAdminEvents" class="accordion-collapse collapse" aria-labelledby="panelHeadingAdminEvents">
                 <div class="accordion-body px-0 py-2">
                     <ul class="nav nav-pills flex-column gap-1">
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
                             {{- mac_sidebar.render_nav_link("Categories", url_for("events.categories.list"), "Manage events categories", ["bi", "bi-tags"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("events.categories.create"), "Add a new event category", ["bi", "bi-plus-circle"]) -}}
                             {% endfilter %}
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
         <div class="accordion-item border-0">
@@ -110,22 +106,20 @@
                 </button>
             </h2>
             <div id="panelCollapseAdminUsers" class="accordion-collapse collapse" aria-labelledby="panelHeadingAdminUsers">
                 <div class="accordion-body px-0 py-2">
                     <ul class="nav nav-pills flex-column gap-1">
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
-                            {{- mac_sidebar.render_nav_link("User groups", url_for("user_groups.list"), "Manage user groups", ["bi", "bi-people-fill"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("user_groups.create"), "Add a new user group", ["bi", "bi-plus-circle"]) -}}
+                            {{- mac_sidebar.render_nav_link("Users", url_for("users.list"), "Manage users", ["bi", "bi-person-lines-fill"], extra_classes=["w-100"]) -}}
                             {% endfilter %}
                         </li>
                         <li class="nav-item d-flex justify-content-between align-items-center gap-1">
                             {% filter indent(width=28, first=True) %}
-                            {{- mac_sidebar.render_nav_link("Users", url_for("users.list"), "Manage users", ["bi", "bi-person-lines-fill"], extra_classes=["w-100"]) -}}
-                            {{- mac_sidebar.render_nav_link(none, url_for("users.create"), "Add a new user", ["bi", "bi-plus-circle"]) -}}
+                            {{- mac_sidebar.render_nav_link("Groups", url_for("user_groups.list"), "Manage groups", ["bi", "bi-people-fill"], extra_classes=["w-100"]) -}}
                             {% endfilter %}
                         </li>
                     </ul>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_analysis.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_analysis.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_services.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_services.html`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             </button>
         </h2>
         <div id="panelCollapseServices" class="accordion-collapse collapse" aria-labelledby="panelHeadingServices">
             <div class="accordion-body px-0 py-2">
                 <ul class="nav nav-pills flex-column gap-1">
                     {% filter indent(width=20, first=True) %}
                     {% if g.campaign_ctxt.has_campaign %}
-                    {{- mac_sidebar.render_nav_item("Cleanup", url_for("services.cleanup.state"), "Cleanup service", ["bi", "bi-magic"]) -}}
+                    {{- mac_sidebar.render_nav_item("Cleanup data", url_for("services.cleanup.state"), "Cleanup data service", ["bi", "bi-magic"]) -}}
                     {{- mac_sidebar.render_nav_item("Check missing data", url_for("services.missing_data.campaign_context_state"), "Check missing data service", ["bi", "bi-journal-x"]) -}}
                     {{- mac_sidebar.render_nav_item("Check outlier data", url_for("services.outlier_data.campaign_context_state"), "Check outlier data service", ["bi", "bi-layout-wtf"]) -}}
                     {{- mac_sidebar.render_nav_item("Weather data", url_for("services.weather_data.manage"), "Weather data service", ["bi", "bi-cloud-sun"]) -}}
                     {% endif %}
                     {% for sidebar_section_plugin in sidebar_section_plugins %}
                     {{- mac_sidebar.render_nav_item_from_plugin(sidebar_section_plugin) -}}
                     {% endfor %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             </button>
         </h2>
         <div id="panelCollapseTSData" class="accordion-collapse collapse" aria-labelledby="panelHeadingTSData">
             <div class="accordion-body px-0 py-2">
                 <ul class="nav nav-pills flex-column gap-1">
                     {% filter indent(width=20, first=True) %}
                     {% if g.campaign_ctxt.has_campaign %}
-                    {{- mac_sidebar.render_nav_item("Explore data", url_for("timeseries.data.explore"), "Explore data", ["bi", "bi-bar-chart-line"]) -}}
+                    {{- mac_sidebar.render_nav_item("Explore timeseries data", url_for("timeseries.data.explore"), "Explore timeseries data", ["bi", "bi-bar-chart-line"]) -}}
                     {{- mac_sidebar.render_nav_item("Data completeness", url_for("timeseries.data.completeness"), "Data completeness", ["bi", "bi-pie-chart"]) -}}
                     {% endif %}
                     {% for sidebar_section_plugin in sidebar_section_plugins %}
                     {{- mac_sidebar.render_nav_item_from_plugin(sidebar_section_plugin) -}}
                     {% endfor %}
                     {% endfilter %}
                 </ul>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/user_group_available.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/user_group_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_available.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_for_group.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_for_group.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/sidebar.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/structural_element_selector.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/structural_element_selector.html`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,14 @@
             </div>
             <app-tree id="treeSelector" ignore-unselect="false" toolbar="{{ treeToolbar | tojson }}" {% if structural_element_types %} types={{ structural_element_types }}{% endif %}></app-tree>
         </div>
     </div>
 </app-structural-element-selector>
 {% endmacro %}
 
-{% macro render_site_selector(html_element_id=none, title="Sites/buildings/... selection") %}
+{% macro render_site_selector(html_element_id=none, title="Sites selection") %}
     {{- _render_structural_element_selector(html_element_id=html_element_id, title=title) }}
 {% endmacro %}
 
 {% macro render_zone_selector(html_element_id=none, title="Zones selection") %}
     {{- _render_structural_element_selector(html_element_id=html_element_id, title=title, structural_element_types="zone", treeToolbar=False) }}
 {% endmacro %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/ts_selector.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/ts_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/macros/flash.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/macros/flash.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/macros/partners.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/macros/partners.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/about.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/about.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/degree_days.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/degree_days.html`

 * *Files 18% similar despite different names*

```diff
@@ -77,22 +77,35 @@
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
-    <div class="row justify-content-center">
+    <div class="row justify-content-center mb-3">
         <div class="col" id="chartContainer">
             <div class="alert alert-info mb-0 pb-0 w-50 mx-auto" role="alert">
                 <span class="fw-bold"><i class="bi bi-question-diamond"></i> Help</span>
                 <p>To see the degree days, <span class="fw-bold">select a site</span> in the tree and <span class="fw-bold">choose a period</span>.</p>
             </div>
         </div>
     </div>
+    <div class="row">
+        <div class="col">
+            <div class="alert alert-info" role="alert">
+                <h5><i class="bi bi-info-square"></i> Degree days calculation</h5>
+                <div><span class="fw-bold">Heating Degree Days</span> (<var>HDD</var>) and <span class="fw-bold">Cooling Degree Days</span> (<var>CDD</var>) are computed with the <span class="fst-italic">mean temperature method</span>.</div>
+                <div class="mb-1">Each day, the average outside air temperature of the day is computed as the mean of min and max temperature (<var>Tmin</var> and <var>Tmax</var>). Then the degree days for that day are computed as the difference between that average temperature and the chosen base temperature (<var>Tbase</var>), taking 0 if negative.</div>
+                <div class="ms-2">
+                    <div><var class="fw-bold">HDD</var> = Max(0, <var>Tbase</var> - (<var>Tmax</var> - <var>Tmin</var>) / 2)</div>
+                    <div><var class="fw-bold">CDD</var> = Max(0, (<var>Tmax</var> - <var>Tmin</var>) / 2 - <var>Tbase</var>)</div>
+                </div>
+            </div>
+        </div>
+    </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
 {% filter indent(width=8, first=True) %}
 <script type="module" src="{{ url_for('static', filename='scripts/modules/views/analysis/degreeDays.js') }}" defer></script>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/energy_consumption.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/energy_consumption.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/weather.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/weather.html`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                                         <div class="d-flex gap-2">
                                             <select id="periodDay" class="form-select d-none invisible" aria-label="Select a period day" required></select>
                                             <select id="periodMonth" class="form-select d-none invisible" aria-label="Select a period month" required></select>
                                             <select id="periodYear" class="form-select d-none invisible" aria-label="Select a period year" required></select>
                                         </div>
                                         <div class="form-check form-switch" id="forecastWrapper">
                                             <input class="form-check-input" type="checkbox" role="switch" id="forecastSwitch">
-                                            <label class="form-check-label text-nowrap" for="forecastSwitch">Show forecast</label>
+                                            <label class="form-check-label text-nowrap" for="forecastSwitch">Show forecast (+ {{ forecast_nbdays }} days)</label>
                                         </div>
                                     </div>
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
@@ -63,33 +63,31 @@
                 </div>
             </div>
         </div>
     </div>
 </div>
 <div class="modal fade" id="tsInfoModal" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="tsInfoModalLabel" aria-hidden="true">
     <div class="modal-dialog modal-lg modal-dialog-centered">
-        <div class="modal-content placeholder-glow">
+        <div class="modal-content">
             <div class="modal-header">
-                <h5 class="modal-title" id="tsInfoModalLabel">Weather parameters timeseries</h5>
+                <h5 class="modal-title" id="tsInfoModalLabel">Weather parameters timeseries - <span id="tsInfoModalChartName"></span></h5>
                 <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
             </div>
-            <div class="modal-body" id="tsInfoModalBody">
-                <div class="tab-content">
-                    <ul class="nav nav-tabs" role="tablist">
-                        <li class="nav-item" role="presentation">
-                            <a href="#current" class="nav-link active" id="current-tab" data-bs-toggle="tab" role="tab" aria-controls="current" aria-selected="true">Current</a>
-                        </li>
-                        <li class="nav-item" role="presentation">
-                            <a href="#forecast" class="nav-link" id="forecast-tab" data-bs-toggle="tab" role="tab" aria-controls="forecast" aria-selected="false">Forecast</a>
-                        </li>
-                    </ul>
-                </div>
-                <div class="tab-content">
-                    <div class="tab-pane fade show active" id="current" role="tabpanel" aria-labelledby="current-tab"></div>
-                    <div class="tab-pane fade" id="forecast" role="tabpanel" aria-labelledby="forecast-tab"></div>
+            <div class="modal-body">
+                <ul class="nav nav-tabs app-tabs" role="tablist">
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link active" id="current-tab" type="button" data-bs-toggle="tab" data-bs-target="#current-tabcontent" role="tab" aria-controls="current-tabcontent" aria-selected="true">Current</button>
+                    </li>
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link" id="forecast-tab" type="button" data-bs-toggle="tab" data-bs-target="#forecast-tabcontent" role="tab" aria-controls="forecast-tabcontent" aria-selected="false">Forecast</button>
+                    </li>
+                </ul>
+                <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white">
+                    <div class="tab-pane fade show active p-3" id="current-tabcontent" role="tabpanel" aria-labelledby="current-tab"></div>
+                    <div class="tab-pane fade p-3" id="forecast-tabcontent" role="tabpanel" aria-labelledby="forecast-tab"></div>
                 </div>
             </div>
             <div class="modal-footer d-flex justify-content-end gap-2">
                 <button type="button" class="btn btn-sm btn-outline-secondary" data-bs-dismiss="modal">Cancel</button>
             </div>
         </div>
     </div>
@@ -101,14 +99,14 @@
 {% filter indent(width=8, first=True) %}
 <script type="module">
     import { WeatherExploreView } from "{{ url_for('static', filename='scripts/modules/views/analysis/weather.js') }}";
 
 
     document.addEventListener("DOMContentLoaded", () => {
 
-        let weatherExploreView = new WeatherExploreView("{{ g.campaign_ctxt.tz_name }}");
+        let weatherExploreView = new WeatherExploreView("{{ g.campaign_ctxt.tz_name }}", {{ forecast_nbdays }});
         weatherExploreView.mount();
 
     });
 </script>
 {% endfilter %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/base.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 <div class="container-fluid h-100">
     <div class="row h-100">
         {% filter indent(width=8, first=True) %}
         {% include "components/sidebar/sidebar.html" %}
         {% endfilter +%}
         <main class="col-md-9 ms-sm-auto col-xl-10 px-md-4 pb-4 app-content">
             {% block main_title %}
-            <div class="d-flex justify-content-between align-items-center gap-3 mb-4">
+            <div class="d-flex justify-content-start align-items-center gap-4 mb-2">
+                {% if title or subtitle %}
                 <div class="d-lg-flex d-grid gap-lg-3">
                     {% if title %}
                     <h1 class="text-nowrap">{{ title }}</h1>
                     {% endif %}
                     {% if subtitle %}
                     <h2 class="align-self-end text-break">{{ subtitle }}</h2>
                     {% endif %}
                 </div>
-                <div class="my-2">
+                {% endif %}
+                <div>
                     {% block main_toolbar %}
                     {% endblock main_toolbar %}
                 </div>
             </div>
             {% endblock main_title %}
             {% filter indent(width=12, first=True) %}
             {% block main_content %}
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
 {% import "macros/flash.html" as mac_flash %} {% extends "pages/skeleton.html"
 %} {% block head_styles %} {{ super() -}} {% filter indent(width=8, first=True)
 %}
  {% endfilter %} {% endblock head_styles %} {% block body_content %} {{ super()
 -}} {% include "components/header.html" +%}
 {% filter indent(width=8, first=True) %} {% include "components/sidebar/
 sidebar.html" %} {% endfilter +%}  {% block main_title %}
+{% if title or subtitle %}
 {% if title %}
 ****** {{ title }} ******
 {% endif %} {% if subtitle %}
 ***** {{ subtitle }} *****
 {% endif %}
+{% endif %}
 {% block main_toolbar %} {% endblock main_toolbar %}
 {% endblock main_title %} {% filter indent(width=12, first=True) %} {% block
 main_content %} {% endblock main_content %} {% endfilter %}
 {{- mac_flash.display_messages() }}
 {% endblock body_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/edit.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
 {% set title = "Campaign scope" %}
 {% set subtitle = "Edit" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
@@ -19,19 +20,16 @@
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5 mb-3">
         <div class="col">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if campaign_scope.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ campaign_scope.campaign_state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ campaign_scope.campaign_name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(campaign_scope.campaign_name, campaign_scope.campaign_state, render_style="bullet") }}
         </div>
         <div class="col">
             <h5>Campaign scope</h5>
             <p class="text-break">{{ campaign_scope.name }}</p>
         </div>
     </div>
     <div class="row">
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-{% extends "pages/base.html" %} {% set title = "Campaign scope" %} {% set
-subtitle = "Edit" %} {% block main_toolbar %} {{ super() -}} {% filter indent
-(width=20, first=True) %}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% set title = "Campaign scope" %} {% set subtitle = "Edit" %} {%
+block main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
 {% set url_back = url_for("campaigns.view", id=campaign_scope.campaign_id,
 tab="scopes") %}
  Back_to_campaign
   Delete
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
 ** Campaign **
-[{{ campaign_scope.campaign_state | upper }}]
-{{ campaign_scope.campaign_name }}
+{{- mac_camp.render_campaign_info(campaign_scope.campaign_name,
+campaign_scope.campaign_state, render_style="bullet") }}
 ** Campaign scope **
 {{ campaign_scope.name }}
  Campaign scope informations
 Name [{{ campaign_scope.name }}]
 Description
 {{ campaign_scope.description }}
 Cancel
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/view.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/view.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
 {% set title = "Campaign scope" %}
 {% if tab is undefined %}
     {% set tab = "general" %}
 {% endif %}
 
 {% block main_toolbar %}
@@ -21,19 +22,16 @@
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5 mb-3">
         <div class="col">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if campaign_scope.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ campaign_scope.campaign_state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ campaign_scope.campaign_name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(campaign_scope.campaign_name, campaign_scope.campaign_state, render_style="bullet") }}
         </div>
     </div>
     <div class="row">
         <div class="col">
             <ul class="nav nav-tabs app-tabs" role="tablist">
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'general' %} active{% endif %}" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tabcontent" type="button" role="tab" aria-controls="general-tabcontent" aria-selected="{% if tab == 'general' %}true{% else %}false{% endif %}">General</button>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-{% extends "pages/base.html" %} {% set title = "Campaign scope" %} {% if tab is
-undefined %} {% set tab = "general" %} {% endif %} {% block main_toolbar %} {
-{ super() -}} {% filter indent(width=20, first=True) %}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% set title = "Campaign scope" %} {% if tab is undefined %} {% set
+tab = "general" %} {% endif %} {% block main_toolbar %} {{ super() -}} {%
+filter indent(width=20, first=True) %}
 {% set url_back = url_for("campaigns.view", id=campaign_scope.campaign_id,
 tab="scopes") %}
  Back_to_campaign
   Delete
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
 ** Campaign **
-[{{ campaign_scope.campaign_state | upper }}]
-{{ campaign_scope.campaign_name }}
+{{- mac_camp.render_campaign_info(campaign_scope.campaign_name,
+campaign_scope.campaign_state, render_style="bullet") }}
     * General
     * User groups {{ user_groups|length }}
   Name
       {{ campaign_scope.name }}
   Description
       {{ campaign_scope.description | default("-", true) }}
 {% if signed_user.is_admin %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/edit.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
 {% set title = "Campaign" %}
 {% set subtitle = "Edit" %}
 
 {% set is_campaign_selected_edit = g.campaign_ctxt.has_campaign and g.campaign_ctxt.id|string == campaign.id|string %}
 
 {% block main_toolbar %}
@@ -14,29 +15,27 @@
 </form>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    {% if is_campaign_selected_edit %}
-    <div class="row mb-3">
-        <div class="col">
+    <div class="row gap-5 mb-4">
+        <div class="col-auto">
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(campaign.name, campaign.state, render_style="bullet") }}
+        </div>
+        {% if is_campaign_selected_edit %}
+        <div class="col-auto">
             <div class="alert alert-info" role="alert">
                 <i class="bi bi-info-square me-2"></i>
                 This is the campaign currently selected. <span class="fw-bold fst-italic">Deletion is disabled.</span>
             </div>
         </div>
-    </div>
-    {% endif %}
-    <div class="row mb-3">
-        <div class="col">
-            <h5>Campaign</h5>
-            <p class="text-break">{{ campaign.name }}</p>
-        </div>
+        {% endif %}
     </div>
     <div class="row">
         <div class="col">
             <fieldset>
                 <legend class="invisible d-none">Campaign information</legend>
                 <div class="mb-3">
                     <label class="form-label" for="name">Name</label>
@@ -45,18 +44,14 @@
                 <div class="mb-3">
                     <label class="form-label" for="timezonePicker">Timezone</label>
                     <div is="app-timezone-picker" id="timezonePicker" input-form-bind="timezone" tzname="{{ campaign.timezone }}" required>
                         <div is="app-spinner"></div>
                     </div>
                     <input form="editForm" type="hidden" id="timezone" name="timezone" value="{{ campaign.timezone }}" required>
                 </div>
-                <div class="mb-3">
-                    <label class="form-label" for="description">Description</label>
-                    <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ campaign.description }}</textarea>
-                </div>
                 <div class="row d-xl-flex d-grid mb-3">
                     <div class="col pb-3 pb-xl-0">
                         <label class="form-label" for="start_datetime">From</label>
                         <div is="app-datetime-picker" id="start_datetime" date-input-form-bind="start_date" time-input-form-bind="start_time" date="{{ campaign.start_date }}" time="{{ campaign.start_time }}">
                             <div is="app-spinner"></div>
                         </div>
                         <input form="editForm" type="hidden" id="start_date" name="start_date" value="{{ campaign.start_date }}">
@@ -67,14 +62,18 @@
                         <div is="app-datetime-picker" id="end_datetime" date-input-form-bind="end_date" time-input-form-bind="end_time" date="{{ campaign.end_date }}" time="{{ campaign.end_time }}">
                             <div is="app-spinner"></div>
                         </div>
                         <input form="editForm" type="hidden" id="end_date" name="end_date" value="{{ campaign.end_date }}">
                         <input form="editForm" type="hidden" id="end_time" name="end_time" value="{{ campaign.end_time }}">
                     </div>
                 </div>
+                <div class="mb-3">
+                    <label class="form-label" for="description">Description</label>
+                    <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ campaign.description }}</textarea>
+                </div>
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('campaigns.view', id=campaign.id) }}" class="btn btn-outline-secondary btn-sm text-break" title="Cancel">Cancel</a>
                     <form id="editForm" action="{{ url_for('campaigns.edit', id=campaign.id) }}" method="POST">
                         <input type="hidden" form="editForm" id="editEtag" name="editEtag" value="{{ etag }}">
                         <button type="submit" form="editForm" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
                     </form>
                 </div>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/list.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
 {% set title = "Campaigns" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
 {% if signed_user.is_admin %}
-<div class="d-sm-flex d-grid gap-3">
-    <a href="{{ url_for('campaign_scopes.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new campaign scope"><i class="bi bi-plus-circle"></i> New campaign scope</a>
-    <div class="vr d-none d-sm-block"></div>
-    <a href="{{ url_for('campaigns.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new campaign"><i class="bi bi-plus-circle"></i> New campaign</a>
-</div>
+<a href="{{ url_for('campaigns.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new campaign"><i class="bi bi-plus-circle"></i> Add</a>
 {% endif %}
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
@@ -52,23 +49,22 @@
         </div>
     </div>
     <div class="row">
         <div class="col">
             <div class="list-group">
                 {% for x in campaigns %}
                 {% set is_campaign_selected = g.campaign_ctxt.has_campaign and g.campaign_ctxt.id|string == x.id|string %}
-                <div class="list-group-item d-flex justify-content-between gap-3 p-0{% if is_campaign_selected %} app-campaign-selected{% endif %}">
+                <div class="list-group-item d-flex justify-content-between gap-3 p-0{% if is_campaign_selected %} border-start border-5 border-top-0 border-end-0 border-bottom-0 app-campaign-selected{% endif %}">
                     <a class="list-group-item-action text-decoration-none d-flex gap-3 py-3 p-2 ps-3 w-100" href="{{ url_for('campaigns.view', id=x.id) }}" title="View details">
                         <i class="bi bi-boxes"></i>
                         <div class="d-xl-flex d-grid justify-content-between gap-3 w-100">
                             <div class="d-grid gap-2">
-                                <div class="d-sm-flex d-grid align-items-center gap-1">
-                                    <small class="fw-bold text-{% if x.state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ x.state | upper }}]</small>
-                                    <h6 class="fw-bold text-break ms-sm-2 mb-0">{{ x.name }}</h6>
-                                </div>
+                                <h6 class="fw-bold">
+                                    {{- mac_camp.render_campaign_info(x.name, x.state, render_style="bullet") }}
+                                </h6>
                                 {% if is_campaign_selected %}
                                 <div><small class="text-opacity-50 text-primary fst-italic"><i class="bi bi-info-square"></i> This campaign is currently selected.</small></div>
                                 {% endif %}
                                 <div class="text-muted ms-2">{{ x.description }}</div>
                             </div>
                             <div class="v-stack">
                                 <div class="d-md-flex d-grid align-items-center gap-md-2">
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
-{% extends "pages/base.html" %} {% set title = "Campaigns" %} {% block
-main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %} {% if
-signed_user.is_admin %}
- New_campaign_scope
- New_campaign
-{% endif %} {% endfilter %} {% endblock main_toolbar %} {% block main_content
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% set title = "Campaigns" %} {% block main_toolbar %} {{ super() -
+}} {% filter indent(width=20, first=True) %} {% if signed_user.is_admin %}
+ Add
+ {% endif %} {% endfilter %} {% endblock main_toolbar %} {% block main_content
 %} {{ super() -}}
   Filters
 % if g.campaign_ctxt.campaign_state_overall == filters["state"] %} selected{%
 endif %}>All campaign states
 {% for x in g.campaign_ctxt.campaign_states %}
 % if x == filters["state"] %} selected{% endif %}>{{ x | capitalize }}
 {% endfor %}
   Apply
  Remove
 {% for x in campaigns %} {% set is_campaign_selected =
 g.campaign_ctxt.has_campaign and g.campaign_ctxt.id|string == x.id|string %}
-[{{_x.state_|_upper_}}]
-*_{{_x.name_}}_*
+*_{{-_mac_camp.render_campaign_info(x.name,_x.state,_render_style="bullet")_}}
+*
 {%_if_is_campaign_selected_%}
  This_campaign_is_currently_selected.
 {%_endif_%}
 {{_x.description_}}
  {{_x.timezone_info["area"]["label"]_}}
 {{_x.timezone_info["label"]_}}
 {%_if_x.start_time_is_defined_%}_{%_set_is_ongoing_=_x.state_==_"ongoing"_%}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/manage_groups.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/manage_groups.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/view.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/create.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create an event category" %}
+{% set title = "New event category" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('events.categories.create') }}" method="POST">
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% extends "pages/base.html" %} {% set title = "Create an event category" %} {%
-block main_content %} {{ super() -}}
+{% extends "pages/base.html" %} {% set title = "New event category" %} {% block
+main_content %} {{ super() -}}
  Event category information
 Name [name                ]
 Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/list.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "pages/base.html" %}
 
 {% set title = "Event categories" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('events.categories.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new event category"><i class="bi bi-plus-circle"></i> New event category</a>
+<a href="{{ url_for('events.categories.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new event category"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row justify-content-end mb-3">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %} {% set title = "Event categories" %} {% block
 main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
- New_event_category
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
 {% for x in event_categories %}
 *_{{_x.name_}}_*
 {{_x.description_}}
  {% endfor %}
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/create.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create an event entry" %}
+{% set title = "New event entry" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('events.create') }}" method="POST">
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% extends "pages/base.html" %}
 
 {% set title = "Events" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('events.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new event entry"><i class="bi bi-plus-circle"></i> New event</a>
+<a href="{{ url_for('events.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new event entry"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-4">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% import "macros/components/structural_element_selector.html" as
 mac_struct_elmt_selector %} {% extends "pages/base.html" %} {% set title =
 "Events" %} {% block main_toolbar %} {{ super() -}} {% filter indent(width=20,
 first=True) %}
- New_event
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
   Filters
 Site/building... selection {% filter indent(width=12, first=False) %} {
 { mac_struct_elmt_selector.render_site_selector(html_element_id="siteSelector",
 title=none) -}} {% endfilter %}
 ⁰ extend search to sub-locations
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/home.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/stats.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                     <div class="d-flex flex-column justify-content-center border rounded p-2" style="transform: rotate(0);">
                         <span class="badge bg-primary rounded-pill mx-auto">{{ ts_count }}</span>
                         <a class="stretched-link text-decoration-none" href="{{ url_for('timeseries.list') }}" title="View timeseries">timeseries</a>
                     </div>
                     {% for struct_elmt_type in structural_element_types %}
                     <div class="d-flex flex-column justify-content-center border rounded p-2" style="transform: rotate(0);">
                         <span class="badge bg-primary rounded-pill mx-auto">{{ structural_element_count[struct_elmt_type] }}</span>
-                        <a class="stretched-link text-decoration-none" href="{{ url_for('structural_elements.explore', tab='sites' if struct_elmt_type != 'zone' else 'zones') }}" title="Explore structural elements">{{ struct_elmt_type }}s</a>
+                        <a class="stretched-link text-decoration-none" href="{{ url_for('structural_elements.explore', tab='sites' if struct_elmt_type != 'zone' else 'zones') }}" title="Explore sites">{{ struct_elmt_type }}s</a>
                     </div>
                     {% endfor %}
                 </div>
             </div>
         </div>
         {% endif %}
         <div class="col">
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/explore.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/setup.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Cleanup service" %}
+{% set title = "Cleanup data service" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
         <div class="col">
             <div class="accordion" id="accordionFilters">
@@ -56,18 +57,17 @@
                 {% elif x.id is not none %}
                     {% set manage_url = url_for("services.cleanup.cleanup_state", id=x.id) %}
                 {% endif %}
                 <a class="list-group-item list-group-item-action d-flex gap-3 py-3{% if is_campaign_selected %} app-campaign-selected{% endif %}" href="{{ manage_url }}" title="Manage campaign cleanup">
                     <i class="bi bi-puzzle"></i>
                     <div class="d-sm-flex d-grid justify-content-between gap-2 w-100">
                         <div class="d-grid gap-2">
-                            <div class="d-flex flex-wrap gap-1">
-                                <small class="fw-bold text-{% if x.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ x.campaign_state | upper }}]</small>
-                                <h6 class="fw-bold text-break ms-2 mb-0">{{ x.campaign_name }}</h6>
-                            </div>
+                            <h6 class="fw-bold">
+                                {{- mac_camp.render_campaign_info(x.campaign_name, x.campaign_state, render_style="bullet") }}
+                            </h6>
                             {% if is_campaign_selected %}
                             <div><small class="text-opacity-50 text-primary text-nowrap fst-italic"><i class="bi bi-info-square"></i> This campaign is currently selected.</small></div>
                             {% endif %}
                         </div>
                         <div class="d-flex flex-sm-column gap-sm-0 gap-3">
                             <span><small class="fw-bold text-nowrap">Cleanup state</small></span>
                             {% if x.is_enabled %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/manage.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/manage.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Cleanup service" %}
+{% if signed_user.is_admin %}
+    {% set title = "Manage cleanup data service" %}
+{% else %}
+    {% set title = "Cleanup data service" %}
+{% endif %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5 mb-3">
         <div class="col">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if cleanup_campaign.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ cleanup_campaign.campaign_state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ cleanup_campaign.campaign_name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(cleanup_campaign.campaign_name, cleanup_campaign.campaign_state, render_style="bullet") }}
         </div>
         <div class="col">
-            <h5>Service state</h5>
+            <h5>Service state (on server)</h5>
             {% if signed_user.is_admin %}
             <input type="radio" class="btn-check" name="svc_state" id="svc_state_on" autocomplete="off"{% if cleanup_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-success" for="svc_state_on">ON</label>
             <input type="radio" class="btn-check" name="svc_state" id="svc_state_off" autocomplete="off"{% if not cleanup_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-danger" for="svc_state_off">OFF</label>
             <input type="hidden" name="cleanup_id" id="cleanup_id"{% if cleanup_campaign.id is not none %} value="{{ cleanup_campaign.id }}"{% endif %}>
             <input type="hidden" name="campaign_id" id="campaign_id"{% if cleanup_campaign.campaign_id is not none %} value="{{ cleanup_campaign.campaign_id }}"{% endif %}>
@@ -31,17 +33,17 @@
             {% endif %}
             {% endif %}
         </div>
     </div>
     <div class="row mb-3">
         <div class="col"> 
             <div class="d-flex justify-content-between align-items-center">
-                <form id="formFiltersElmt" class="d-lg-flex d-grid gap-2" action="{{ url_for(request.endpoint, **request.view_args) }}" method="POST">
+                <form id="formFiltersElmt" class="d-lg-flex d-grid align-items-center gap-2" action="{{ url_for(request.endpoint, **request.view_args) }}" method="POST">
                     <input type="hidden" name="sort" id="sort" value="{{ sort }}">
-                    <label class="form-label text-nowrap text-muted mb-0" for="sort">Sort by</label>
+                    <label class="form-label text-nowrap text-muted mb-0" for="sort"><small>Sort by</small></label>
                     <input type="radio" class="btn-check" name="sort" id="sort-timeseries_name-asc" autocomplete="off" {% if sort == "+timeseries_name" %} checked{% endif %}>
                     <label class="btn btn-sm btn-outline-info" for="sort-timeseries_name-asc" title="Name alphabetical order"><i class="bi bi-sort-alpha-down"></i> Name</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-timeseries_name-desc" autocomplete="off" {% if sort == "-timeseries_name" %} checked{% endif %}>
                     <label class="btn btn-sm btn-outline-info" for="sort-timeseries_name-desc" title="Name reverse alphabetical order"><i class="bi bi-sort-alpha-up"></i> Name</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-last_timestamp-asc" autocomplete="off"{% if sort == "+last_timestamp" %} checked{% endif %}>
                     <label class="btn btn-sm btn-outline-info" for="sort-last_timestamp-asc" title="Timestamp date order"><i class="bi bi-sort-numeric-down"></i> Timestamp</label>
                     <input type="radio" class="btn-check" name="sort" id="sort-last_timestamp-desc" autocomplete="off"{% if sort == "-last_timestamp" %} checked{% endif %}>
@@ -88,13 +90,11 @@
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
-{% if signed_user.is_admin %}
 {% filter indent(width=8, first=True) %}
 <script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/cleanupManage.js') }}"></script>
 {% endfilter %}
-{% endif %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
 {% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/missingData/list.js') }}"></script>
+<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/missingData/list.js') }}" defer></script>
 {% endfilter %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/manage.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/manage.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Check missing data service" %}
+{% if signed_user.is_admin %}
+    {% set title = "Manage check outlier data service" %}
+{% else %}
+    {% set title = "Check outlier data service" %}
+{% endif %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5">
         <div class="col">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if missing_data_campaign.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ missing_data_campaign.campaign_state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ missing_data_campaign.campaign_name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(outlier_data_campaign.campaign_name, outlier_data_campaign.campaign_state, render_style="bullet") }}
         </div>
         <div class="col">
-            <h5>Service state</h5>
+            <h5>Service state (on server)</h5>
             {% if signed_user.is_admin %}
-            <input type="radio" class="btn-check" name="svc_state" id="svc_state_on" autocomplete="off"{% if missing_data_campaign.is_enabled %} checked{% endif %}>
+            <input type="radio" class="btn-check" name="svc_state" id="svc_state_on" autocomplete="off"{% if outlier_data_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-success" for="svc_state_on">ON</label>
-            <input type="radio" class="btn-check" name="svc_state" id="svc_state_off" autocomplete="off"{% if not missing_data_campaign.is_enabled %} checked{% endif %}>
+            <input type="radio" class="btn-check" name="svc_state" id="svc_state_off" autocomplete="off"{% if not outlier_data_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-danger" for="svc_state_off">OFF</label>
-            <input type="hidden" name="campaign_service_id" id="campaign_service_id"{% if missing_data_campaign.id is not none %} value="{{ missing_data_campaign.id }}"{% endif %}>
-            <input type="hidden" name="campaign_id" id="campaign_id"{% if missing_data_campaign.campaign_id is not none %} value="{{ missing_data_campaign.campaign_id }}"{% endif %}>
+            <input type="hidden" name="campaign_service_id" id="campaign_service_id"{% if outlier_data_campaign.id is not none %} value="{{ outlier_data_campaign.id }}"{% endif %}>
+            <input type="hidden" name="campaign_id" id="campaign_id"{% if outlier_data_campaign.campaign_id is not none %} value="{{ outlier_data_campaign.campaign_id }}"{% endif %}>
             <input type="hidden" name="etag" id="etag" value="{{ etag }}">
             {% else %}
-            {% if missing_data_campaign.is_enabled %}
+            {% if outlier_data_campaign.is_enabled %}
             <span class="fw-bold text-success text-opacity-75">ON</span>
             {% else %}
             <span class="fw-bold text-danger text-opacity-75">OFF</span>
             {% endif %}
             {% endif %}
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
-{% if signed_user.is_admin %}
 {% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/missingData/manage.js') }}"></script>
+<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/outlierData/manage.js') }}" defer></script>
 {% endfilter %}
-{% endif %}
 {% endblock body_scripts %}
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-{% extends "pages/base.html" %} {% set title = "Check missing data service" %}
-{% block main_content %} {{ super() -}}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% if signed_user.is_admin %} {% set title = "Manage check outlier
+data service" %} {% else %} {% set title = "Check outlier data service" %} {%
+endif %} {% block main_content %} {{ super() -}}
 ** Campaign **
-[{{ missing_data_campaign.campaign_state | upper }}]
-{{ missing_data_campaign.campaign_name }}
-** Service state **
+{{- mac_camp.render_campaign_info(outlier_data_campaign.campaign_name,
+outlier_data_campaign.campaign_state, render_style="bullet") }}
+** Service state (on server) **
 {% if signed_user.is_admin %}
-% if missing_data_campaign.is_enabled %} checked{% endif %}> ON
-% if not missing_data_campaign.is_enabled %} checked{% endif %}> OFF
-% if missing_data_campaign.id is not none %} value="{{ missing_data_campaign.id
+% if outlier_data_campaign.is_enabled %} checked{% endif %}> ON
+% if not outlier_data_campaign.is_enabled %} checked{% endif %}> OFF
+% if outlier_data_campaign.id is not none %} value="{{ outlier_data_campaign.id
 }}"{% endif %}>
-% if missing_data_campaign.campaign_id is not none %} value="{
-{ missing_data_campaign.campaign_id }}"{% endif %}>  {% else %} {% if
-missing_data_campaign.is_enabled %} ON {% else %} OFF {% endif %} {% endif %}
-{% endblock main_content %} {% block body_scripts %} {{ super() -}} {% if
-signed_user.is_admin %} {% filter indent(width=8, first=True) %}
- {% endfilter %} {% endif %} {% endblock body_scripts %}
+% if outlier_data_campaign.campaign_id is not none %} value="{
+{ outlier_data_campaign.campaign_id }}"{% endif %}>  {% else %} {% if
+outlier_data_campaign.is_enabled %} ON {% else %} OFF {% endif %} {% endif %}
+{% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
+indent(width=8, first=True) %}
+ {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/list.html`

 * *Files 0% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
 {% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/outlierData/list.js') }}"></script>
+<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/outlierData/list.js') }}" defer></script>
 {% endfilter %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/manage.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/manage.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Check outlier data service" %}
+{% if signed_user.is_admin %}
+    {% set title = "Manage check missing data service" %}
+{% else %}
+    {% set title = "Check missing data service" %}
+{% endif %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5">
         <div class="col">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if outlier_data_campaign.campaign_state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ outlier_data_campaign.campaign_state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ outlier_data_campaign.campaign_name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(missing_data_campaign.campaign_name, missing_data_campaign.campaign_state, render_style="bullet") }}
         </div>
         <div class="col">
-            <h5>Service state</h5>
+            <h5>Service state (on server)</h5>
             {% if signed_user.is_admin %}
-            <input type="radio" class="btn-check" name="svc_state" id="svc_state_on" autocomplete="off"{% if outlier_data_campaign.is_enabled %} checked{% endif %}>
+            <input type="radio" class="btn-check" name="svc_state" id="svc_state_on" autocomplete="off"{% if missing_data_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-success" for="svc_state_on">ON</label>
-            <input type="radio" class="btn-check" name="svc_state" id="svc_state_off" autocomplete="off"{% if not outlier_data_campaign.is_enabled %} checked{% endif %}>
+            <input type="radio" class="btn-check" name="svc_state" id="svc_state_off" autocomplete="off"{% if not missing_data_campaign.is_enabled %} checked{% endif %}>
             <label class="btn btn-outline-danger" for="svc_state_off">OFF</label>
-            <input type="hidden" name="campaign_service_id" id="campaign_service_id"{% if outlier_data_campaign.id is not none %} value="{{ outlier_data_campaign.id }}"{% endif %}>
-            <input type="hidden" name="campaign_id" id="campaign_id"{% if outlier_data_campaign.campaign_id is not none %} value="{{ outlier_data_campaign.campaign_id }}"{% endif %}>
+            <input type="hidden" name="campaign_service_id" id="campaign_service_id"{% if missing_data_campaign.id is not none %} value="{{ missing_data_campaign.id }}"{% endif %}>
+            <input type="hidden" name="campaign_id" id="campaign_id"{% if missing_data_campaign.campaign_id is not none %} value="{{ missing_data_campaign.campaign_id }}"{% endif %}>
             <input type="hidden" name="etag" id="etag" value="{{ etag }}">
             {% else %}
-            {% if outlier_data_campaign.is_enabled %}
+            {% if missing_data_campaign.is_enabled %}
             <span class="fw-bold text-success text-opacity-75">ON</span>
             {% else %}
             <span class="fw-bold text-danger text-opacity-75">OFF</span>
             {% endif %}
             {% endif %}
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
 {% block body_scripts %}
 {{ super() -}}
 {% if signed_user.is_admin %}
 {% filter indent(width=8, first=True) %}
-<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/outlierData/manage.js') }}"></script>
+<script type="module" src="{{ url_for('static', filename='scripts/modules/views/services/missingData/manage.js') }}" defer></script>
 {% endfilter %}
 {% endif %}
 {% endblock body_scripts %}
```

#### html2text {}

```diff
@@ -1,17 +1,19 @@
-{% extends "pages/base.html" %} {% set title = "Check outlier data service" %}
-{% block main_content %} {{ super() -}}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% if signed_user.is_admin %} {% set title = "Manage check missing
+data service" %} {% else %} {% set title = "Check missing data service" %} {%
+endif %} {% block main_content %} {{ super() -}}
 ** Campaign **
-[{{ outlier_data_campaign.campaign_state | upper }}]
-{{ outlier_data_campaign.campaign_name }}
-** Service state **
+{{- mac_camp.render_campaign_info(missing_data_campaign.campaign_name,
+missing_data_campaign.campaign_state, render_style="bullet") }}
+** Service state (on server) **
 {% if signed_user.is_admin %}
-% if outlier_data_campaign.is_enabled %} checked{% endif %}> ON
-% if not outlier_data_campaign.is_enabled %} checked{% endif %}> OFF
-% if outlier_data_campaign.id is not none %} value="{{ outlier_data_campaign.id
+% if missing_data_campaign.is_enabled %} checked{% endif %}> ON
+% if not missing_data_campaign.is_enabled %} checked{% endif %}> OFF
+% if missing_data_campaign.id is not none %} value="{{ missing_data_campaign.id
 }}"{% endif %}>
-% if outlier_data_campaign.campaign_id is not none %} value="{
-{ outlier_data_campaign.campaign_id }}"{% endif %}>  {% else %} {% if
-outlier_data_campaign.is_enabled %} ON {% else %} OFF {% endif %} {% endif %}
+% if missing_data_campaign.campaign_id is not none %} value="{
+{ missing_data_campaign.campaign_id }}"{% endif %}>  {% else %} {% if
+missing_data_campaign.is_enabled %} ON {% else %} OFF {% endif %} {% endif %}
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% if
 signed_user.is_admin %} {% filter indent(width=8, first=True) %}
  {% endfilter %} {% endif %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/manage.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/manage.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Weather data service" %}
+{% if signed_user.is_admin %}
+    {% set title = "Manage weather data service" %}
+{% else %}
+    {% set title = "Weather data service" %}
+{% endif %}
 
 {% if not tab %}
     {% set tab = "weather" %}
 {% endif %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row g-5 mb-3">
         <div class="col-auto">
-            <div class="d-flex align-items-start gap-3">
-                <h5>Campaign</h5>
-                <span class="fw-bold text-{% if g.campaign_ctxt.campaign.state == 'ongoing' %}success{% else %}danger{% endif %} text-opacity-75">[{{ g.campaign_ctxt.campaign.state | upper }}]</span>
-            </div>
-            <p class="text-break">{{ g.campaign_ctxt.name }}</p>
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") }}
         </div>
         <div class="col">
             <div class="alert alert-info border border-info mb-0" role="alert">
                 <i class="bi bi-info-square me-1"></i>
                 For each site, {% if signed_user.is_admin %}by using the ON/OFF buttons below, {% endif %}weather data can be fetched automatically from <a href="https://oikolab.com/" target="_blank">oikolab</a> web service.
                 {% if signed_user.is_admin %}
                 <p class="mb-0">You can also do it manually using the fetch data button (<i class="bi bi-cloud-download text-primary"></i>), weither the automatic fetch service is enabled or not.</p>
@@ -64,15 +66,15 @@
                         <table class="table table-sm table-hover caption-top">
                             <caption class="text-end">
                                 <small class="text-nowrap text-muted"><app-items-count id="weatherItemsCount"></app-items-count></small>
                             </caption>
                             <thead>
                                 <tr>
                                     <th scope="col">Site</th>
-                                    <th scope="col">State</th>
+                                    <th scope="col">Service state (on server)</th>
                                     {% if signed_user.is_admin %}
                                     <th scope="col">Fetch data</th>
                                     {% endif %}
                                 </tr>
                             </thead>
                             <tbody class="table-group-divider" id="weatherServiceStatesContainer">
                             </tbody>
@@ -84,15 +86,15 @@
                         <table class="table table-sm table-hover caption-top">
                             <caption class="text-end">
                                 <small class="text-nowrap text-muted"><app-items-count id="weatherForecastItemsCount"></app-items-count></small>
                             </caption>
                             <thead>
                                 <tr>
                                     <th scope="col">Site</th>
-                                    <th scope="col">State</th>
+                                    <th scope="col">Service state (on server)</th>
                                 </tr>
                             </thead>
                             <tbody class="table-group-divider" id="weatherForecastServiceStatesContainer">
                             </tbody>
                         </table>
                     </div>
                 </div>
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-{% extends "pages/base.html" %} {% set title = "Weather data service" %} {% if
-not tab %} {% set tab = "weather" %} {% endif %} {% block main_content %} {
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% if signed_user.is_admin %} {% set title = "Manage weather data
+service" %} {% else %} {% set title = "Weather data service" %} {% endif %} {%
+if not tab %} {% set tab = "weather" %} {% endif %} {% block main_content %} {
 { super() -}}
 ** Campaign **
-[{{ g.campaign_ctxt.campaign.state | upper }}]
-{{ g.campaign_ctxt.name }}
+{{- mac_camp.render_campaign_info(g.campaign_ctxt.name,
+g.campaign_ctxt.campaign.state, render_style="bullet") }}
  For each site, {% if signed_user.is_admin %}by using the ON/OFF buttons below,
 {% endif %}weather data can be fetched automatically from oikolab web service.
 {% if signed_user.is_admin %}
 You can also do it manually using the fetch data button (), weither the
 automatic fetch service is enabled or not.
 {% endif %}
   Filters
 [                    ]
  Remove
     * Weather
     * Weather forecast
-Site State Fetch data
-Site State
+Site Service state (on server) Fetch data
+Site Service state (on server)
 {% if signed_user.is_admin %}
 ** Fetch weather data **
 (excluded from the interval)
 Cancel  Fetch
 {% endif %} {% endblock main_content %} {% block body_scripts %} {{ super() -}}
 {% filter indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/signin.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/signin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/skeleton.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/skeleton.html`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <title>BEMServer{% if title %} - {{ title }}{% if subtitle %} - {{ subtitle }}{% endif %}{% endif %}</title>
         <meta name="description" content="{{ description | default('') }}">
         <meta name="author" content="{{ author | default('Nobatek/INEF4', true) }}">
         <link rel="icon" href="{{ url_for('static', filename='images/bemserver.ico') }}">
         {% block head_styles %}
-        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">
-        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css">
+        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
+        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css">
         <link rel="stylesheet" media="all" href="{{ url_for('static', filename='styles/main.css') }}">
         {% endblock head_styles %}
         {% block head_scripts %}
         {% endblock head_scripts %}
     </head>
     <body>
         {% filter indent(width=8, first=True) %}
         {% block body_content %}
         {% endblock body_content %}
         {% endfilter %}
         {% block body_scripts %}
-        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>
+        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz" crossorigin="anonymous"></script>
         {% endblock body_scripts %}
     </body>
 </html>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/create.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create a new " + type %}
+{% set title = "New " + type %}
 {% set has_no_parents = parent_type is not none and parents|length <= 0 %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     {% if has_no_parents %}
     <div class="row mb-3">
@@ -23,15 +23,15 @@
                 <fieldset{% if has_no_parents %} disabled{% endif %}>
                     <legend class="invisible d-none">{{ type|capitalize }} general informations</legend>
                     {% if parent_type is not none and parents|length > 0 %}
                     <div class="mb-3">
                         <label class="form-label" for="{{ parent_type }}">{{ parent_type|capitalize }}</label>
                         <select class="form-select" id="{{ parent_type }}" name="{{ parent_type }}" aria-label="Select a {{ parent_type }}" required>
                             {% for x in parents %}
-                            <option value="{{ x.id }}">{{ x.name }}</option>
+                            <option value="{{ x.id }}">{{ x.full_path }}</option>
                             {% endfor %}
                         </select>
                     </div>
                     {% endif %}
                     <div class="mb-3">
                         <label class="form-label" for="name">Name</label>
                         <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-{% extends "pages/base.html" %} {% set title = "Create a new " + type %} {% set
+{% extends "pages/base.html" %} {% set title = "New " + type %} {% set
 has_no_parents = parent_type is not none and parents|length <= 0 %} {% block
 main_content %} {{ super() -}}
 {% if has_no_parents %}
  Your campaign currently has no {{ parent_type }}s. You must first create_a_{
 {_parent_type_}} to add a {{ type }} to it.
 {% endif %}
 % if has_no_parents %} disabled{% endif %}> {{ type|capitalize }} general
 informations {% if parent_type is not none and parents|length > 0 %}
 {% for x in parents %}
-{{ x.name }}
+{{ x.full_path }}
 {% endfor %}
 {% endif %}
 Name [name                ]
 {% if type == 'site' %}
 Latitude [Â°] [Unknown INPUT type]
 Longitude [Â°] [Unknown INPUT type]
 {% endif %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/edit.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = type|capitalize %}
+{% set title = "Timeseries" %}
 {% set subtitle = "Edit" %}
 
-{% set url_create_property = url_for('structural_elements.properties.create', type=type, back=url_for('structural_elements.edit', type=type, id=structural_element.id, tab='properties')|urlencode) %}
+{% if tab is undefined %}
+    {% set tab = "general" %}
+{% endif %}
+
+{% set url_create_property = url_for('timeseries.properties.create', back=url_for('timeseries.edit', id=timeseries.id, tab='properties')|urlencode) %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<form id="delForm" action="{{ url_for('structural_elements.delete', type=type, id=structural_element.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ structural_element.name }}&lt;/mark&gt; {{ type }}">
+<form id="delForm" action="{{ url_for('timeseries.delete', id=timeseries.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ timeseries.name }}&lt;/mark&gt; timeseries">
     <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
-    <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
+    <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash me-1"></i>Delete</button>
 </form>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    <div class="row mb-3">
+    <div class="row g-5 mb-3">
+        <div class="col-auto">
+            <h5>Campaign</h5>
+            {{- mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") }}
+        </div>
+        <div class="col">
+            <h5>Campaign scope</h5>
+            <p>{{ timeseries.campaign_scope_name }}</p>
+        </div>
+    </div>
+    <div class="row">
         <div class="col">
             <ul class="nav nav-tabs app-tabs" role="tablist">
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'general' %} active{% endif %}" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tabcontent" type="button" role="tab" aria-controls="general-tabcontent" aria-selected="{% if tab == 'general' %}true{% else %}false{% endif %}">General</button>
                 </li>
                 <li class="nav-item" role="presentation">
-                    <button class="nav-link{% if tab == 'properties' %} active{% endif %}" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="{% if tab == 'properties' %}true{% else %}false{% endif %}">Properties <span class="badge bg-secondary">{{ properties|length }}</span></button>
+                    <button class="nav-link{% if tab == 'attributes' %} active{% endif %}" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="{% if tab == 'attributes' %}true{% else %}false{% endif %}">Attributes <span class="badge bg-secondary">{{ properties|length }}</span></button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white mb-3">
                 <div class="tab-pane fade{% if tab == 'general' %} show active{% endif %} p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab">
                     <fieldset>
-                        <legend class="invisible d-none">{{ type|capitalize }} general informations</legend>
+                        <legend class="invisible d-none">Timeseries general information</legend>
                         <div class="mb-3">
                             <label class="form-label" for="name">Name</label>
-                            <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ structural_element.name }}" minlength="1" maxlength="80" required autofocus>
+                            <input type="text" form="editForm" class="form-control" id="name" name="name" minlength="1" maxlength="80" value="{{ timeseries.name }}" required autofocus>
                         </div>
-                        {% if type == "site" %}
-                        <div class="row mb-3">
-                            <div class="col">
-                                <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
-                                <input type="number" form="editForm" class="form-control hide-arrows" id="latitude" name="latitude" min="-90" max="90" step="any" value="{{ structural_element.latitude }}">
-                            </div>
-                            <div class="col">
-                                <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
-                                <input type="number" form="editForm" class="form-control hide-arrows" id="longitude" name="longitude" min="-180" max="180" step="any" value="{{ structural_element.longitude }}">
-                            </div>
-                        </div>
-                        {% endif %}
                         <div class="mb-3">
                             <label class="form-label" for="description">Description</label>
-                            <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ structural_element.description }}</textarea>
+                            <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ timeseries.description }}</textarea>
                         </div>
                         <div class="mb-3">
-                            <label class="form-label" for="ifc_id">IFC ID</label>
-                            <input type="text" form="editForm" class="form-control" id="ifc_id" name="ifc_id" value="{{ structural_element.ifc_id }}" maxlength="22">
+                            <label class="form-label" for="unit_symbol">Unit symbol</label>
+                            <input type="text" form="editForm" class="form-control" id="unit_symbol" name="unit_symbol" maxlength="20" value="{{ timeseries.unit_symbol }}">
                         </div>
                     </fieldset>
                 </div>
-                <div class="tab-pane fade{% if tab == 'properties' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
+                <div class="tab-pane fade{% if tab == 'attributes' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
                     <fieldset>
-                        <legend class="invisible d-none">{{ type|capitalize }} properties</legend>
+                        <legend class="invisible d-none">Timeseries attributes</legend>
                         {% for property_id, property_data in properties.items() %}
                         <div class="mb-3">
                             <label class="form-label" for="property-{{ property_id }}">{{ property_data.name }}{% if property_data.unit_symbol %}<span class="fst-italic text-muted ms-1">[{{ property_data.unit_symbol }}]</span>{% endif %}</label>
                             <input type="hidden" form="editForm" class="form-control" id="property-{{ property_id }}-etag" name="property-{{ property_id }}-etag" value="{{ property_data.etag }}">
                             <div class="d-flex justify-content-between align-items-top gap-3">
                                 <div class="w-100">
                                     {% if property_data.value_type == "boolean" %}
@@ -72,61 +75,61 @@
                                         <input type="checkbox"{% if property_data.value == "true" %} checked{% endif %} form="editForm" class="form-check-input" role="switch" id="property-{{ property_id }}" name="property-{{ property_id }}">
                                     </div>
                                     {% else %}
                                     <input {% if property_data.value_type == "string" %}type="text" maxlength="100"{% elif property_data.value_type in ["integer", "float"] %}type="number"{% if property_data.value_type == "float" %} step="0.01"{% endif %}{% endif %} form="editForm" class="form-control" id="property-{{ property_id }}" name="property-{{ property_id }}" value="{{ property_data.value }}" required>
                                     {% endif %}
                                     <small class="fst-italic text-muted">{{ [property_data.description, property_data.value_type] | select | join(", ") }}</small>
                                 </div>
-                                <form class="mt-1" id="delPropertyForm-{{ property_data.id }}" action="{{ url_for('structural_elements.delete_property', type=type, id=structural_element.id, property_id=property_data.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property_data.name }}&lt;/mark&gt; property">
+                                <form class="mt-1" id="delPropertyForm-{{ property_data.id }}" action="{{ url_for('timeseries.delete_property', id=timeseries.id, property_id=property_data.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property_data.name }}&lt;/mark&gt; attribute">
                                     <input type="hidden" form="delPropertyForm-{{ property_data.id }}" id="delPropertyEtag-{{ property_data.id }}" name="delPropertyEtag-{{ property_data.id }}" value="{{ property_data.etag }}">
-                                    <button type="submit" form="delPropertyForm-{{ property_data.id }}" class="btn btn-sm btn-outline-danger" title="Delete property"><i class="bi bi-trash"></i></button>
+                                    <button type="submit" form="delPropertyForm-{{ property_data.id }}" class="btn btn-sm btn-outline-danger" title="Delete attribute"><i class="bi bi-trash"></i></button>
                                 </form>
                             </div>
                         </div>
                         {% endfor %}
                         <div class="d-flex justify-content-center mb-3">
                             {% if available_properties|length > 0 %}
                             <div class="dropdown">
                                 <button class="btn btn-sm btn-outline-primary dropdown-toggle" type="button" id="addPropertyBtn" data-bs-toggle="dropdown" aria-expanded="false">
-                                    <i class="bi bi-plus-circle"></i> Define a property
+                                    <i class="bi bi-plus-circle"></i> Define an attribute
                                 </button>
-                                <ul class="dropdown-menu" aria-labelledby="addPropertyBtn">
-                                    <li><a class="dropdown-item" role="button" data-bs-toggle="modal" data-bs-target="#addProperty">Choose from available properties ({{ available_properties|length }})</a></li>
-                                    <li><a class="dropdown-item" href="{{ url_create_property }}">Create a new property</a></li>
+                                <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
+                                    <li><a class="dropdown-item" role="button" data-bs-toggle="modal" data-bs-target="#addProperty">Choose from available attributes ({{ available_properties|length }})</a></li>
+                                    <li><a class="dropdown-item" href="{{ url_create_property }}">Create a new attribute</a></li>
                                 </ul>
                             </div>
                             {% else %}
-                            <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new property"><i class="bi bi-plus-circle"></i> Add a new property</a>
+                            <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new attribute"><i class="bi bi-plus-circle"></i> Add a new attribute</a>
                             {% endif %}
                         </div>
                     </fieldset>
                 </div>
             </div>
             <div class="d-flex justify-content-end gap-2">
-                <a href="{{ url_for('structural_elements.explore') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
-                <form id="editForm" action="{{ url_for('structural_elements.edit', type=type, id=structural_element.id) }}" method="POST">
+                <a href="{{ url_for('timeseries.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
+                <form id="editForm" action="{{ url_for('timeseries.edit', id=timeseries.id) }}" method="POST">
                     <input type="hidden" form="editForm" id="editEtag" name="editEtag" value="{{ etag }}">
-                    <button type="submit" form="editForm" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
+                    <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save me-1"></i>Save</button>
                 </form>
             </div>
         </div>
     </div>
 </div>
 <div class="modal fade" id="addProperty" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="addPropertyLabel" aria-hidden="true">
     <div class="modal-dialog modal-lg modal-dialog-centered">
         <div class="modal-content">
             <div class="modal-header">
-                <h5 class="modal-title" id="addPropertyLabel">Define a property</h5>
+                <h5 class="modal-title" id="addPropertyLabel">Define an attribute</h5>
                 <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
             </div>
             <div class="modal-body">
-                <form id="addPropertyForm" action="{{ url_for('structural_elements.create_property', type=type, id=structural_element.id) }}" method="POST">
+                <form id="addPropertyForm" action="{{ url_for('timeseries.create_property', id=timeseries.id) }}" method="POST">
                     <div class="mb-3">
-                        <label class="form-label" for="availableProperty">Available properties <span class="badge bg-secondary">{{ available_properties|length }}</span></label>
-                        <select form="addPropertyForm" class="form-select" id="availableProperty" name="availableProperty" aria-label="Select a property">
+                        <label class="form-label" for="availableProperty">Available attributes <span class="badge bg-secondary">{{ available_properties|length }}</span></label>
+                        <select form="addPropertyForm" class="form-select" id="availableProperty" name="availableProperty" aria-label="Select an attribute">
                             {% for property_id, property_data in available_properties.items() %}
                             <option value="{{ property_id }}" data-property-type="{{ property_data.value_type }}" data-property-description="{{ property_data.description }}"{% if loop.first %} selected{% endif %}>{{ property_data.name }}{% if property_data.unit_symbol %} [{{ property_data.unit_symbol }}]{% endif %}</option>
                             {% endfor %}
                         </select>
                     </div>
                     <div class="mb-3" id="availablePropertyInputContainer">
                         <input type="hidden" class="form-control" form="addPropertyForm" id="availablePropertyValueType" name="availablePropertyValueType">
@@ -134,18 +137,18 @@
                             <input class="form-control" form="addPropertyForm" id="availablePropertyValue" name="availablePropertyValue">
                         </div>
                         <small class="fst-italic text-muted" id="availablePropertyDescription"></small>
                     </div>
                 </form>
             </div>
             <div class="modal-footer d-flex justify-content-between">
-                <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new property"><i class="bi bi-plus-circle"></i> Add a new property</a>
+                <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new attribute"><i class="bi bi-plus-circle me-1"></i>Add a new attribute</a>
                 <div>
                     <button type="button" class="btn btn-sm btn-outline-secondary" data-bs-dismiss="modal">Cancel</button>
-                    <button type="submit" form="addPropertyForm" class="btn btn-sm btn-primary"><i class="bi bi-save"></i> Save</button>
+                    <button type="submit" form="addPropertyForm" class="btn btn-sm btn-primary"><i class="bi bi-save me-1"></i>Save</button>
                 </div>
             </div>
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
@@ -157,14 +160,15 @@
     document.addEventListener("DOMContentLoaded", () => {
 
         let availablePropertySelectElmt = document.getElementById("availableProperty");
         let availablePropertyInputContainerElmt = document.getElementById("availablePropertyInputContainer");
         let availablePropertyInputElmt = document.getElementById("availablePropertyValue");
         let availablePropertyValueTypeElmt = document.getElementById("availablePropertyValueType");
         let availablePropertyDescriptionElmt = document.getElementById("availablePropertyDescription");
+        let addPropertyModalElmt = document.getElementById("addProperty");
 
         function updatePropertyDescription() {
             if (availablePropertySelectElmt.selectedIndex != -1) {
                 let selectedProperty = availablePropertySelectElmt.selectedOptions[0];
                 let propertyType = selectedProperty.getAttribute("data-property-type", "string");
 
                 availablePropertyInputElmt.removeAttribute("readonly");
@@ -196,28 +200,33 @@
                         availablePropertyInputElmt.classList.replace("form-control", "form-check-input");
                         availablePropertyInputElmt.type = "checkbox";
                         availablePropertyInputElmt.setAttribute("role", "switch");
                         availablePropertyInputElmt.parentElement.classList.add("form-check", "form-switch");
                         break;
                 }
 
+                availablePropertyInputElmt.focus();
+
                 availablePropertyDescriptionElmt.innerHTML = [selectedProperty.getAttribute("data-property-description"), propertyType].filter(Boolean).join(", ");
             }
             else {
                 availablePropertyInputElmt.setAttribute("readonly", true);
                 availablePropertyDescriptionElmt.innerHTML = "";
             }
         }
 
-        if (availablePropertySelectElmt.selectedIndex != -1) {
+        availablePropertySelectElmt.addEventListener("change", () => {
             updatePropertyDescription();
-        }
-        availablePropertySelectElmt.addEventListener("change", (event) => {
-            event.preventDefault();
+        });
 
-            updatePropertyDescription();
+        addPropertyModalElmt.addEventListener("shown.bs.modal", () => {
+            availablePropertyInputElmt.focus();
         });
 
+        if (availablePropertySelectElmt.selectedIndex != -1) {
+            updatePropertyDescription();
+        }
+
     });
 </script>
 {% endfilter %}
 {% endblock body_scripts %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/explore.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/explore.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,146 @@
 {% extends "pages/base.html" %}
 
 {% set title = "Explore sites" %}
 
+{% block main_toolbar %}
+{{ super() -}}
+{% filter indent(width=20, first=True) %}
+{% if signed_user.is_admin %}
+<div class="d-none d-sm-flex gap-2">
+    <div class="btn-group">
+        <button id="dropdownAddSites" type="button" class="btn btn-sm btn-outline-primary text-nowrap dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" title="Add a new site/building/sotrey/space or zone"><i class="bi bi-plus-circle"></i> Add</button>
+        <ul class="dropdown-menu" aria-labelledby="dropdownAddSites">
+            <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='site') }}" title="Add a new site">Site</a></li>
+            <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='building') }}" title="Add a new building">Building</a></li>
+            <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='storey') }}" title="Add a new storey">Storey</a></li>
+            <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='space') }}" title="Add a new space">Space</a></li>
+            <li><hr class="dropdown-divider"></li>
+            <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='zone') }}" title="Add a new zone">Zone</a></li>
+        </ul>
+    </div>
+    <div class="vr mx-1"></div>
+    <a class="btn btn-sm btn-outline-success text-nowrap" href="{{ url_for('structural_elements.upload') }}" title="Import CSV files"><i class="bi bi-upload"></i> Import CSV</a>
+</div>
+<div class="btn-group d-sm-none">
+    <button id="dropdownActions" type="button" class="btn btn-sm btn-outline-primary text-nowrap dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" title="Manage sites"><i class="bi bi-three-dots-vertical"></i> Actions</button>
+    <ul class="dropdown-menu" aria-labelledby="dropdownActions">
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='site') }}" title="Add a new site">New site</a></li>
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='building') }}" title="Add a new building">New building</a></li>
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='storey') }}" title="Add a new storey">New storey</a></li>
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='space') }}" title="Add a new space">New space</a></li>
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.create', type='zone') }}" title="Add a new zone">New zone</a></li>
+        <li><hr class="dropdown-divider"></li>
+        <li><a class="dropdown-item" href="{{ url_for('structural_elements.upload') }}" title="Import CSV files">Import CSV</a></li>
+    </ul>
+</div>
+{% endif %}
+{% endfilter %}
+{% endblock main_toolbar %}
+
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    <div class="row d-xl-flex d-grid mb-3 mb-xl-0 h-100">
+    <div class="row d-xl-flex d-grid h-100">
         <div class="col col-xl-6 pb-3 pb-xl-0">
             <ul class="nav nav-tabs app-tabs" id="tabSites" role="tablist">
                 <li class="nav-item" role="presentation">
-                    <button class="nav-link{% if tab == 'sites' %} active{% endif %}" id="sites-tab" data-bs-toggle="tab" data-bs-target="#sites-tabcontent" type="button" role="tab" aria-controls="sites-tabcontent" aria-selected="{% if tab == 'sites' %}true{% else %}false{% endif %}"><i class="bi bi-buildings"></i> Sites / Buildings...</button>
+                    <button class="nav-link{% if tab == 'sites' %} active{% endif %}" id="sites-tab" data-bs-toggle="tab" data-bs-target="#sites-tabcontent" type="button" role="tab" aria-controls="sites-tabcontent" aria-selected="{% if tab == 'sites' %}true{% else %}false{% endif %}"><i class="bi bi-buildings me-1"></i>Sites</button>
                 </li>
                 <li class="nav-item" role="presentation">
-                    <button class="nav-link{% if tab == 'zones' %} active{% endif %}" id="zones-tab" data-bs-toggle="tab" data-bs-target="#zones-tabcontent" type="button" role="tab" aria-controls="zones-tabcontent" aria-selected="{% if tab == 'zones' %}true{% else %}false{% endif %}"><i class="bi bi-bullseye"></i> Zones</button>
+                    <button class="nav-link{% if tab == 'zones' %} active{% endif %}" id="zones-tab" data-bs-toggle="tab" data-bs-target="#zones-tabcontent" type="button" role="tab" aria-controls="zones-tabcontent" aria-selected="{% if tab == 'zones' %}true{% else %}false{% endif %}"><i class="bi bi-bullseye me-1"></i>Zones</button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white" id="tabSitesContent">
                 <div class="tab-pane fade{% if tab == 'sites' %} show active{% endif %} p-3" id="sites-tabcontent" role="tabpanel" aria-labelledby="sites-tab">
                     <app-tree id="sitesTree"></app-tree>
                 </div>
                 <div class="tab-pane fade{% if tab == 'zones' %} show active{% endif %} p-3" id="zones-tabcontent" role="tabpanel" aria-labelledby="zones-tab">
                     <app-tree id="zonesTree" toolbar="false"></app-tree>
                 </div>
             </div>
         </div>
         <div class="col">
-            <ul class="nav nav-tabs app-tabs" id="tabProperties" role="tablist">
-                <li class="nav-item" role="presentation">
-                    <button class="nav-link active" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tabcontent" type="button" role="tab" aria-controls="general-tabcontent" aria-selected="true">General</button>
-                </li>
-                <li class="nav-item" role="presentation">
-                    <button class="nav-link" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="false">Properties</button>
-                </li>
-                <li class="nav-item" role="presentation">
-                    <button class="nav-link" id="timeseries-tab" data-bs-toggle="tab" data-bs-target="#timeseries-tabcontent" type="button" role="tab" aria-controls="timeseries-tabcontent" aria-selected="false">Timeseries</button>
-                </li>
-                <li class="nav-item" role="presentation">
-                    <button class="nav-link" id="events-tab" data-bs-toggle="tab" data-bs-target="#events-tabcontent" type="button" role="tab" aria-controls="events-tabcontent" aria-selected="false">Events</button>
-                </li>
-            </ul>
-            <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white" id="tabPropertiesContent">
-                <div class="tab-pane fade show active p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab"></div>
-                <div class="tab-pane fade p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab"></div>
-                <div class="tab-pane fade p-3" id="timeseries-tabcontent" role="tabpanel" aria-labelledby="timeseries-tab">
-                    <div class="row mb-1">
-                        <div class="col">
-                            <div class="form-check form-switch">
-                                <input class="form-check-input" type="checkbox" role="switch" id="tsRecurseSwitch">
-                                <label class="form-check-label" for="tsRecurseSwitch">extend search to sub-locations</label>
+            <div id="alertInfoData" class="alert alert-info" role="alert">
+                <i class="bi bi-info-square float-start me-2"></i>
+                <span>Select a <span class="fw-bold">site/building/storey/space or zone</span> in the tree to explore its data.</span>
+            </div>
+            <div id="selectedStructutalElementInfoContainer" class="d-none invisible">
+                <h5 class="text-secondary">Information about selected <span id="selectedStructuralElementType">element</span></h5>
+                <ul class="nav nav-tabs app-tabs" id="tabData" role="tablist">
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link active" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tabcontent" type="button" role="tab" aria-controls="general-tabcontent" aria-selected="true">General</button>
+                    </li>
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="false">Attributes</button>
+                    </li>
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link" id="timeseries-tab" data-bs-toggle="tab" data-bs-target="#timeseries-tabcontent" type="button" role="tab" aria-controls="timeseries-tabcontent" aria-selected="false">Timeseries</button>
+                    </li>
+                    <li class="nav-item" role="presentation">
+                        <button class="nav-link" id="events-tab" data-bs-toggle="tab" data-bs-target="#events-tabcontent" type="button" role="tab" aria-controls="events-tabcontent" aria-selected="false">Events</button>
+                    </li>
+                </ul>
+                <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white" id="tabDataContent">
+                    <div class="tab-pane fade show active p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab"></div>
+                    <div class="tab-pane fade p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab"></div>
+                    <div class="tab-pane fade p-3" id="timeseries-tabcontent" role="tabpanel" aria-labelledby="timeseries-tab">
+                        <div class="row mb-1">
+                            <div class="col">
+                                <div class="form-check form-switch">
+                                    <input class="form-check-input" type="checkbox" role="switch" id="tsRecurseSwitch">
+                                    <label class="form-check-label" for="tsRecurseSwitch">extend search to sub-locations</label>
+                                </div>
                             </div>
                         </div>
-                    </div>
-                    <div class="row mb-3">
-                        <div class="d-flex align-items-center gap-2">
-                            <label class="form-label m-0" for="search">Search</label>
-                            <input type="text" class="form-control form-control-sm" id="tsSearch" name="tsSearch" placeholder="Name..." autofocus>
-                            <a id="tsClear" role="button" class="link-danger text-decoration-none mx-1 d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
+                        <div class="row mb-3">
+                            <div class="d-flex align-items-center gap-2">
+                                <label class="form-label m-0" for="search">Search</label>
+                                <input type="text" class="form-control form-control-sm" id="tsSearch" name="tsSearch" placeholder="Name..." autofocus>
+                                <a id="tsClear" role="button" class="link-danger text-decoration-none mx-1 d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
+                            </div>
                         </div>
+                        <nav class="row" aria-label="Timeseries pagination">
+                            <div class="col-auto align-self-center py-1">
+                                <div is="app-pagesize-selector" id="tsPageSize"></div>
+                            </div>
+                            <div class="col d-flex flex-wrap justify-content-end align-items-center gap-2">
+                                <small class="text-nowrap text-muted"><app-items-count id="tsCount"></app-items-count></small>
+                                <ul is="app-pagination" id="tsPagination"></ul>
+                            </div>
+                        </nav>
+                        <div id="tsList" class="list-group py-2"></div>
                     </div>
-                    <nav class="row" aria-label="Timeseries pagination">
-                        <div class="col-auto align-self-center py-1">
-                            <div is="app-pagesize-selector" id="tsPageSize"></div>
-                        </div>
-                        <div class="col d-flex flex-wrap justify-content-end align-items-center gap-2">
-                            <small class="text-nowrap text-muted"><app-items-count id="tsCount"></app-items-count></small>
-                            <ul is="app-pagination" id="tsPagination"></ul>
-                        </div>
-                    </nav>
-                    <div id="tsList" class="list-group py-2"></div>
-                </div>
-                <div class="tab-pane fade p-3" id="events-tabcontent" role="tabpanel" aria-labelledby="events-tab">
-                    <div class="row mb-1">
-                        <div class="col">
-                            <div class="form-check form-switch">
-                                <input class="form-check-input" type="checkbox" role="switch" id="eventsRecurseSwitch">
-                                <label class="form-check-label" for="eventsRecurseSwitch">extend search to sub-locations</label>
+                    <div class="tab-pane fade p-3" id="events-tabcontent" role="tabpanel" aria-labelledby="events-tab">
+                        <div class="row mb-1">
+                            <div class="col">
+                                <div class="form-check form-switch">
+                                    <input class="form-check-input" type="checkbox" role="switch" id="eventsRecurseSwitch">
+                                    <label class="form-check-label" for="eventsRecurseSwitch">extend search to sub-locations</label>
+                                </div>
                             </div>
                         </div>
-                    </div>
-                    <div class="row mb-3">
-                        <div class="d-flex align-items-center gap-2">
-                            <label class="form-label m-0" for="search">Search</label>
-                            <input type="text" class="form-control form-control-sm" id="eventsSearch" name="eventsSearch" placeholder="Source..." autofocus>
-                            <a id="eventsClear" role="button" class="link-danger text-decoration-none mx-1 d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
+                        <div class="row mb-3">
+                            <div class="d-flex align-items-center gap-2">
+                                <label class="form-label m-0" for="search">Search</label>
+                                <input type="text" class="form-control form-control-sm" id="eventsSearch" name="eventsSearch" placeholder="Source..." autofocus>
+                                <a id="eventsClear" role="button" class="link-danger text-decoration-none mx-1 d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
+                            </div>
                         </div>
+                        <nav class="row" aria-label="Events pagination">
+                            <div class="col-auto align-self-center py-1">
+                                <div is="app-pagesize-selector" id="eventsPageSize"></div>
+                            </div>
+                            <div class="col d-flex flex-wrap justify-content-end align-items-center gap-2">
+                                <small class="text-nowrap text-muted"><app-items-count id="eventsCount"></app-items-count></small>
+                                <ul is="app-pagination" id="eventsPagination"></ul>
+                            </div>
+                        </nav>
+                        <div id="eventsList" class="list-group py-2"></div>
                     </div>
-                    <nav class="row" aria-label="Events pagination">
-                        <div class="col-auto align-self-center py-1">
-                            <div is="app-pagesize-selector" id="eventsPageSize"></div>
-                        </div>
-                        <div class="col d-flex flex-wrap justify-content-end align-items-center gap-2">
-                            <small class="text-nowrap text-muted"><app-items-count id="eventsCount"></app-items-count></small>
-                            <ul is="app-pagination" id="eventsPagination"></ul>
-                        </div>
-                    </nav>
-                    <div id="eventsList" class="list-group py-2"></div>
                 </div>
             </div>
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
@@ -112,13 +154,13 @@
     document.addEventListener("DOMContentLoaded", () => {
 
         let options = {
             timezone: {{ g.campaign_ctxt.tz_name | tojson }},
         };
 
         let structuralElmts = new StructuralElementsExploreView(options);
-        structuralElmts.refresh();
+        structuralElmts.mount();
 
     });
 </script>
 {% endfilter %}
 {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/create.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create a new structural element property" %}
+{% set title = "New sites attribute" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('structural_elements.properties.create', next=url_cancel) }}" method="POST">
                 <fieldset>
-                    <legend class="invisible d-none">Structural element property informations</legend>
-                    <div class="mb-3">
-                        <label class="form-label" for="name">Name</label>
-                        <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
-                    </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="value_type">Type</label>
-                        <select class="form-select" id="value_type" name="value_type" aria-label="Select a value" required>
-                            <option value="integer">integer</option>
-                            <option value="float">float</option>
-                            <option value="boolean">boolean</option>
-                            <option value="string">string</option>
-                        </select>
+                    <legend class="invisible d-none">Sites attribute information</legend>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="name">Name</label>
+                            <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
+                        </div>
                     </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="unit_symbol">Unit symbol</label>
-                        <input type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20">
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="value_type">Type</label>
+                            <select class="form-select" id="value_type" name="value_type" aria-label="Select a value" required>
+                                {% for x in property_value_types %}
+                                <option value="{{ x.name }}">{{ x.value }}</option>
+                                {% endfor %}
+                            </select>
+                        </div>
+                        <div class="col">
+                            <label class="form-label" for="unit_symbol">Unit symbol</label>
+                            <input type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20">
+                        </div>
                     </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="description">Description</label>
-                        <textarea class="form-control" id="description" name="description" maxlength="500" rows="3"></textarea>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="description">Description</label>
+                            <textarea class="form-control" id="description" name="description" maxlength="500" rows="3"></textarea>
+                        </div>
                     </div>
-                    <div class="mb-3">
-                        <p>Add this property for</p>
-                        <div class="d-flex flex-wrap gap-2">
-                            {% for x in structural_elements %}
-                            <div class="form-check form-switch me-4">
-                                <input class="form-check-input" type="checkbox" role="switch" id="{{ x }}" name="{{ x }}">
-                                <label class="form-check-label" for="{{ x }}">{{ x | capitalize }}</label>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <h5>Make this attribute available for the following levels:</h5>
+                            <div class="d-flex flex-wrap gap-2">
+                                {% for x in structural_elements %}
+                                <div class="form-check form-switch me-4">
+                                    <input class="form-check-input" type="checkbox" role="switch" id="{{ x }}" name="{{ x }}">
+                                    <label class="form-check-label" for="{{ x }}">{{ x | capitalize }}</label>
+                                </div>
+                                {% endfor %}
                             </div>
-                            {% endfor %}
                         </div>
                     </div>
                     <div class="d-flex justify-content-end gap-2">
                         <a href="{{ url_cancel }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                         <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
                     </div>
                 </fieldset>
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-{% extends "pages/base.html" %} {% set title = "Create a new structural element
-property" %} {% block main_content %} {{ super() -}}
- Structural element property informations
+{% extends "pages/base.html" %} {% set title = "New sites attribute" %} {%
+block main_content %} {{ super() -}}
+ Sites attribute information
 Name [name                ]
-Type [One of: integer/float/boolean/string]
+{% for x in property_value_types %}
+{{ x.value }}
+{% endfor %}
 Unit symbol [unit_symbol         ]
-Add this property for
+** Make this attribute available for the following levels: **
 {% for x in structural_elements %}
 ⁰ {{ x | capitalize }}
 {% endfor %}
 Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Structural element property" %}
+{% set title = "Sites attribute" %}
 {% set subtitle = "Edit" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<form id="delForm" action="{{ url_for('structural_elements.properties.delete', id=property.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property.name }}&lt;/mark&gt; property">
+<form id="delForm" action="{{ url_for('structural_elements.properties.delete', id=property.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property.name }}&lt;/mark&gt; attribute">
     <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
     <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
 </form>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <fieldset>
-                <legend class="invisible d-none">Structural element property informations</legend>
-                <div class="mb-3">
-                    <label class="form-label" for="name">Name</label>
-                    <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ property.name }}" minlength="1" maxlength="80" required autofocus>
-                </div>
-                <div class="mb-3">
-                    <label class="form-label" for="value_type">Type</label>
-                    <input type="text" class="form-control" id="value_type" name="value_type" value="{{ property.value_type }}" readonly>
+                <legend class="invisible d-none">Sites attribute information</legend>
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="name">Name</label>
+                        <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ property.name }}" minlength="1" maxlength="80" required autofocus>
+                    </div>
                 </div>
-                <div class="mb-3">
-                    <label class="form-label" for="unit_symbol">Unit symbol</label>
-                    <input form="editForm" type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20" value="{{ property.unit_symbol }}">
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="value_type">Type</label>
+                        <input type="text" class="form-control" id="value_type" name="value_type" value="{{ property.value_type }}" disabled readonly>
+                    </div>
+                    <div class="col">
+                        <label class="form-label" for="unit_symbol">Unit symbol</label>
+                        <input form="editForm" type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20" value="{{ property.unit_symbol }}">
+                    </div>
                 </div>
-                <div class="mb-3">
-                    <label class="form-label" for="description">Description</label>
-                    <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ property.description }}</textarea>
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="description">Description</label>
+                        <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ property.description }}</textarea>
+                    </div>
                 </div>
                 {% if structural_elements|length > 0 %}
-                <div class="mb-3">
-                    <h5>Add this property for</h5>
-                    <div class="d-flex flex-wrap gap-2">
-                        {% for struct_elmt in structural_elements %}
-                        <div class="form-check form-switch me-4">
-                            <input class="form-check-input" type="checkbox" form="editForm" role="switch" id="{{ struct_elmt }}" name="{{ struct_elmt }}"{% if property.used_in[struct_elmt] %} checked{% endif %}>
-                            <label class="form-check-label" for="{{ struct_elmt }}">{{ struct_elmt | capitalize }}</label>
+                <div class="row mb-3">
+                    <div class="col">
+                        <h5>Make this attribute available for the following levels:</h5>
+                        <div class="d-flex flex-wrap gap-2">
+                            {% for struct_elmt in structural_elements %}
+                            <div class="form-check form-switch me-4">
+                                <input class="form-check-input" type="checkbox" form="editForm" role="switch" id="{{ struct_elmt }}" name="{{ struct_elmt }}"{% if property.used_in[struct_elmt] %} checked{% endif %}>
+                                <label class="form-check-label" for="{{ struct_elmt }}">{{ struct_elmt | capitalize }}</label>
+                            </div>
+                            {% endfor %}
                         </div>
-                        {% endfor %}
                     </div>
                 </div>
                 {% endif %}
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('structural_elements.properties.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                     <form id="editForm" action="{{ url_for('structural_elements.properties.edit', id=property.id) }}" method="POST">
                         <input type="hidden" form="editForm" id="editEtag" name="editEtag" value="{{ etag }}">
                         <button type="submit" form="editForm" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
-                    </form>    
+                    </form>
                 </div>
             </fieldset>
         </div>
     </div>
 </div>
 {% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-{% extends "pages/base.html" %} {% set title = "Structural element property" %}
-{% set subtitle = "Edit" %} {% block main_toolbar %} {{ super() -}} {% filter
-indent(width=20, first=True) %}
+{% extends "pages/base.html" %} {% set title = "Sites attribute" %} {% set
+subtitle = "Edit" %} {% block main_toolbar %} {{ super() -}} {% filter indent
+(width=20, first=True) %}
   Delete
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
- Structural element property informations
+ Sites attribute information
 Name [{{ property.name }} ]
 Type [{{ property.value_type }}]
 Unit symbol [{{ property.unit_symbol }}]
 Description
 {{ property.description }}
 {% if structural_elements|length > 0 %}
-** Add this property for **
+** Make this attribute available for the following levels: **
 {% for struct_elmt in structural_elements %}
 % if property.used_in[struct_elmt] %} checked{% endif %}> {{ struct_elmt |
 capitalize }}
 {% endfor %}
 {% endif %}
 Cancel
   Save
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Structural elements properties" %}
+{% set title = "Sites attributes" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('structural_elements.properties.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new property"><i class="bi bi-plus-circle"></i> New property</a>
+<a href="{{ url_for('structural_elements.properties.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new attribute"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
@@ -53,15 +53,15 @@
                 <table class="table table-sm table-hover table-bordered caption-top">
                     <caption class="text-end">
                         <small class="text-nowrap text-muted"><app-items-count id="itemCount" first-item="{% if properties | length > 0 %}1{% else %}0{% endif %}" last-item="{{ properties | length }}" total-count="{{ total_count }}"></app-items-count></small>
                     </caption>
                     <thead>
                         <tr>
                             <th scope="col" colspan="4"></th>
-                            <th scope="col" colspan="{{ structural_elements|length }}" class="text-center">Used in</th>
+                            <th scope="col" colspan="{{ structural_elements|length }}" class="text-center">Available for the following levels</th>
                             <th scope="col"></th>
                         </tr>
                         <tr>
                             <th scope="col" class="w-25">Name</th>
                             <th scope="col">Type</th>
                             <th scope="col">Unit</th>
                             <th scope="col" class="w-25">Description</th>
@@ -89,15 +89,15 @@
                                 {% if prop.used_in[struct_elmt] %}
                                 <span class="text-success"><i class="bi bi-hand-thumbs-up"></i> yes</span>
                                 {% else %}
                                 <span class="text-danger"><i class="bi bi-hand-thumbs-down"></i> no</span>
                                 {% endif %}
                             </td>
                             {% endfor %}
-                            <td class="text-center"><a class="btn btn-sm btn-outline-secondary" href="{{ url_for('structural_elements.properties.edit', id=prop.id) }}" title="Edit property"><i class="bi bi-pencil"></i></td>
+                            <td class="text-center"><a class="btn btn-sm btn-outline-secondary" href="{{ url_for('structural_elements.properties.edit', id=prop.id) }}" title="Edit attribute"><i class="bi bi-pencil"></i></td>
                         </tr>
                         {% endfor %}
                     </tbody>
                 </table>
             </div>
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-{% extends "pages/base.html" %} {% set title = "Structural elements properties"
-%} {% block main_toolbar %} {{ super() -}} {% filter indent(width=20,
-first=True) %}
- New_property
+{% extends "pages/base.html" %} {% set title = "Sites attributes" %} {% block
+main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
   Filters
 {% for struct_elmt in structural_elements %}
 % if filters[struct_elmt] %} checked{% endif %}> {{ struct_elmt | capitalize }}
 {% endfor %}
 % if filters["orphan"] %} checked{% endif %}> Orphan
  Apply
  Remove
-                                                                   Used in
+                                                                   Available for
+                                                                   the following
+                                                                   levels
                                                                    {
 Name      Type            Unit             Description             { struct_elmt
                                                                    | capitalize
                                                                    }}s
                                            {% if                   {% if
 {         {               {                prop.description|length prop.used_in
 {         {               {                > 80 %} {               [struct_elmt]
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/upload.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/create.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Upload sites" %}
+{% set title = "New user" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    <div class="row mb-3">
-        <div class="col">
-            <h5>Campaign</h5>
-            <p class="text-break">{{ g.campaign_ctxt.name }}</p>
-        </div>
-    </div>
     <div class="row">
         <div class="col">
-            <form action="{{ url_for('structural_elements.upload') }}" enctype="multipart/form-data" method="POST">
+            <form action="{{ url_for('users.create') }}" method="POST">
                 <fieldset>
-                    <legend class="invisible d-none">Sites data files</legend>
-                    {% for struct_elmt_type in structural_element_types %}
+                    <legend class="invisible d-none">User account information</legend>
+                    <div class="mb-3">
+                        <label class="form-label" for="name">Name</label>
+                        <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
+                    </div>
+                    <div class="mb-3">
+                        <label class="form-label" for="email">Email address</label>
+                        <input type="email" class="form-control" id="email" name="email" required>
+                    </div>
                     <div class="mb-3">
-                        <label class="form-label" for="{{ struct_elmt_type }}s_csv"><span class="fw-bold">{{ struct_elmt_type | capitalize }}s</span> CSV file</label>
-                        <input type="file" class="form-control" id="{{ struct_elmt_type }}s_csv" name="{{ struct_elmt_type }}s_csv" accept=".csv" aria-label="Select a CSV file"{% if loop.index == 1%} autofocus{% endif %}>
+                        <label class="form-label" for="password">Password</label>
+                        <input type="password" class="form-control" id="password" name="password" minlength="1" maxlength="80" required>
                     </div>
-                    {% endfor %}
                     <div class="d-flex justify-content-end gap-2">
-                        <a href="{{ url_for('main.index') }}" class="btn btn-sm btn-outline-secondary" title="Cancel">Cancel</a>
-                        <button type="submit" class="btn btn-sm btn-primary" title="Upload file"><i class="bi bi-upload"></i> Upload</button>
+                        <a href="{{ url_for('users.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
+                        <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
                     </div>
                 </fieldset>
             </form>
         </div>
     </div>
 </div>
 {% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,10 +1,8 @@
-{% extends "pages/base.html" %} {% set title = "Upload sites" %} {% block
+{% extends "pages/base.html" %} {% set title = "New user" %} {% block
 main_content %} {{ super() -}}
-** Campaign **
-{{ g.campaign_ctxt.name }}
- Sites data files {% for struct_elmt_type in structural_element_types %}
-{{ struct_elmt_type | capitalize }}s CSV file
-% if loop.index == 1%} autofocus{% endif %}>
-{% endfor %}
-Cancel  Upload
+ User account information
+Name [name                ]
+Email address [Unknown INPUT type]
+Password [********************]
+Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/create.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
 
-{% set title = "Create a new timeseries" %}
+{% set title = "New timeseries" %}
 
 {% set has_campaign_scopes = campaign_scopes|length > 0 %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     {% if not has_campaign_scopes %}
@@ -17,15 +18,15 @@
             </div>
         </div>
     </div>
     {% endif %}
     <div class="row mb-3">
         <div class="col">
             <h5>Campaign</h5>
-            <p class="text-break">{{ g.campaign_ctxt.name }}</p>
+            {{- mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") }}
         </div>
     </div>
     <div class="row">
         <div class="col">
             <form action="{{ url_for('timeseries.create') }}" method="POST">
                 <fieldset{% if not has_campaign_scopes %} disabled{% endif %}>
                     <legend class="invisible d-none">Timeseries informations</legend>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-{% extends "pages/base.html" %} {% set title = "Create a new timeseries" %} {%
-set has_campaign_scopes = campaign_scopes|length > 0 %} {% block main_content
-%} {{ super() -}}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% set title = "New timeseries" %} {% set has_campaign_scopes =
+campaign_scopes|length > 0 %} {% block main_content %} {{ super() -}}
 {% if not has_campaign_scopes %}
  Selected campaign has currently no campaign scopes. You must first create_a
 campaign_scope to add a timeseries to it.
 {% endif %}
 ** Campaign **
-{{ g.campaign_ctxt.name }}
+{{- mac_camp.render_campaign_info(g.campaign_ctxt.name,
+g.campaign_ctxt.campaign.state, render_style="bullet") }}
 % if not has_campaign_scopes %} disabled{% endif %}> Timeseries informations
 {% for x in campaign_scopes %}
 {{ x.name }}
 {% endfor %}
 Name [name                ]
 Unit symbol [unit_symbol         ]
 Cancel
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/completeness.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/completeness.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/delete.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/delete.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-{% import "macros/components/ts_selector.html" as mac_ts_selector %}
 {% extends "pages/base.html" %}
+{% import "macros/components/campaign.html" as mac_camp %}
+{% import "macros/components/ts_selector.html" as mac_ts_selector %}
 
 {% set title = "Delete timeseries data" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
@@ -11,18 +12,18 @@
             <div class="alert alert-warning border border-warning" role="alert">
                 <h4 class="alert-heading"><i class="bi bi-exclamation-triangle"></i> Warning</h4>
                 <p>You are about to <span class="fw-bold">delete timeseries data</span>!</p>
                 <p class="mb-0">Keep in mind that <span class="fw-bold">data can not be restored</span> once this operation is done.</p>
             </div>
         </div>
     </div>
-    <div class="row mb-3">
-        <div class="col">
+    <div class="row g-5 mb-3">
+        <div class="col-auto">
             <h5>Campaign</h5>
-            <p>{{ g.campaign_ctxt.name }}</p>
+            {{- mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") }}
         </div>
     </div>
     <div class="row mb-3">
         <div class="col">
             {% filter indent(width=12, first=False) %}
             {{ mac_ts_selector.render_ts_selector(element_id="tsSelectorDelete") -}}
             {% endfilter %}
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-{% import "macros/components/ts_selector.html" as mac_ts_selector %} {% extends
-"pages/base.html" %} {% set title = "Delete timeseries data" %} {% block
-main_content %} {{ super() -}}
+{% extends "pages/base.html" %} {% import "macros/components/campaign.html" as
+mac_camp %} {% import "macros/components/ts_selector.html" as mac_ts_selector
+%} {% set title = "Delete timeseries data" %} {% block main_content %} {{ super
+() -}}
  Warning
 You are about to delete timeseries data!
 Keep in mind that data can not be restored once this operation is done.
 ** Campaign **
-{{ g.campaign_ctxt.name }}
+{{- mac_camp.render_campaign_info(g.campaign_ctxt.name,
+g.campaign_ctxt.campaign.state, render_style="bullet") }}
 {% filter indent(width=12, first=False) %} {
 { mac_ts_selector.render_ts_selector(element_id="tsSelectorDelete") -}} {%
 endfilter %}
 (excluded from the interval)
  Delete
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/explore.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/upload.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/list.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Upload timeseries data" %}
+{% set title = "Timeseries data states" %}
+
+{% block main_toolbar %}
+{{ super() -}}
+{% filter indent(width=20, first=True) %}
+<a href="{{ url_for('timeseries.datastates.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new timeseries data state"><i class="bi bi-plus-circle"></i> Add</a>
+{% endfilter %}
+{% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
-    <div class="row mb-3">
-        <h5>Campaign</h5>
-        <p>{{ g.campaign_ctxt.name }}</p>
+    <div class="row justify-content-end mb-3">
+        <div class="col-auto">
+            <small class="text-nowrap text-muted"><app-items-count first-item="1" last-item="{{ timeseries_datastates | length }}" total-count="{{ timeseries_datastates | length }}"></app-items-count></small>
+        </div>
     </div>
     <div class="row">
         <div class="col">
-            <form action="{{ url_for('timeseries.data.upload') }}" enctype="multipart/form-data" method="POST">
-                <fieldset>
-                    <legend class="invisible d-none">Timeseries data files</legend>
-                    <div class="mb-3">
-                        <label class="form-label" for="data_state">Timeseries data state</label>
-                        <select class="form-select" id="data_state" name="data_state" aria-label="Select a timeseries data state" required>
-                            {% for x in ts_datastates %}
-                            <option value="{{ x.id }}">{{ x.name }}</option>
-                            {% endfor %}
-                        </select>
-                    </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="csv_file">Select a CSV file</label>
-                        <input type="file" class="form-control" id="csv_file" name="csv_file" accept=".csv" aria-label="Select a CSV file" required autofocus>
-                    </div>
-                    <div class="d-flex justify-content-end gap-2">
-                        <a href="{{ url_for('main.index') }}" class="btn btn-sm btn-outline-secondary" title="Cancel">Cancel</a>
-                        <button type="submit" class="btn btn-sm btn-primary" title="Upload file"><i class="bi bi-upload"></i> Upload</button>
-                    </div>
-                </fieldset>
-            </form>
+            <div class="list-group">
+                {% for x in timeseries_datastates %}
+                <a class="list-group-item list-group-item-action d-flex align-items-center gap-3 py-3" href="{{ url_for('timeseries.datastates.edit', id=x.id) }}" title="Edit">
+                    <i class="bi bi-tag"></i>
+                    <h6 class="fw-bold text-break mb-0">{{ x.name }}</h6>
+                </a>
+                {% endfor %}
+            </div>
         </div>
     </div>
 </div>
-{% endblock main_content %}
+{% endblock main_content %}
+
+{% block body_scripts %}
+{{ super() -}}
+{% filter indent(width=8, first=True) %}
+<script type="module" src="{{ url_for('static', filename='scripts/modules/components/itemsCount.js') }}"></script>
+{% endfilter %}
+{% endblock body_scripts %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "pages/base.html" %} {% set title = "Upload timeseries data" %} {%
-block main_content %} {{ super() -}}
-** Campaign **
-{{ g.campaign_ctxt.name }}
- Timeseries data files
-{% for x in ts_datastates %}
-{{ x.name }}
-{% endfor %}
-Select a CSV file [File]
-Cancel  Upload
-{% endblock main_content %}
+{% extends "pages/base.html" %} {% set title = "Timeseries data states" %} {%
+block main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
+ Add
+ {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
+() -}}
+{% for x in timeseries_datastates %}
+*_{{_x.name_}}_*
+ {% endfor %}
+{% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
+indent(width=8, first=True) %}
+ {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create a timeseries data state" %}
+{% set title = "New timeseries data state" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('timeseries.datastates.create') }}" method="POST">
                 <fieldset>
-                    <legend class="invisible d-none">Timeseries data states informations</legend>
+                    <legend class="invisible d-none">Timeseries data state information</legend>
                     <div class="mb-3">
                         <label class="form-label" for="name">Name</label>
                         <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
                     </div>
                     <div class="d-flex justify-content-end gap-2">
                         <a href="{{ url_for('timeseries.datastates.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                         <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% extends "pages/base.html" %} {% set title = "Create a timeseries data state"
-%} {% block main_content %} {{ super() -}}
- Timeseries data states informations
+{% extends "pages/base.html" %} {% set title = "New timeseries data state" %}
+{% block main_content %} {{ super() -}}
+ Timeseries data state information
 Name [name                ]
 Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/list.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Timeseries data states" %}
+{% set title = "Groups" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('timeseries.datastates.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new timeseries data state"><i class="bi bi-plus-circle"></i> New data state</a>
+<a href="{{ url_for('user_groups.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new group"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row justify-content-end mb-3">
         <div class="col-auto">
-            <small class="text-nowrap text-muted"><app-items-count first-item="1" last-item="{{ timeseries_datastates | length }}" total-count="{{ timeseries_datastates | length }}"></app-items-count></small>
+            <small class="text-nowrap text-muted"><app-items-count first-item="1" last-item="{{ user_groups | length }}" total-count="{{ user_groups | length }}"></app-items-count></small>
         </div>
     </div>
     <div class="row">
         <div class="col">
             <div class="list-group">
-                {% for x in timeseries_datastates %}
-                <a class="list-group-item list-group-item-action d-flex align-items-center gap-3 py-3" href="{{ url_for('timeseries.datastates.edit', id=x.id) }}" title="Edit">
-                    <i class="bi bi-inbox"></i>
-                    <h6 class="fw-bold text-break mb-0">{{ x.name }}</h6>
+                {% for x in user_groups %}
+                <a class="list-group-item list-group-item-action d-flex gap-3 py-3" href="{{ url_for('user_groups.view', id=x.id) }}" title="View group">
+                    <i class="bi bi-person-rolodex"></i>
+                    <div class="d-flex gap-2 w-100 justify-content-between">
+                        <div>
+                            <h6 class="fw-bold mb-0">{{ x.name }}</h6>
+                        </div>
+                    </div>
                 </a>
                 {% endfor %}
             </div>
         </div>
     </div>
 </div>
 {% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "pages/base.html" %} {% set title = "Timeseries data states" %} {%
-block main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
- New_data_state
+{% extends "pages/base.html" %} {% set title = "Groups" %} {% block
+main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
-{% for x in timeseries_datastates %}
+{% for x in user_groups %}
 *_{{_x.name_}}_*
  {% endfor %}
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/edit.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Timeseries" %}
+{% set title = type|capitalize %}
 {% set subtitle = "Edit" %}
 
-{% set url_create_property = url_for('timeseries.properties.create', back=url_for('timeseries.edit', id=timeseries.id, tab='properties')|urlencode) %}
+{% if tab is undefined %}
+    {% set tab = "general" %}
+{% endif %}
+
+{% set url_create_property = url_for('structural_elements.properties.create', type=type, back=url_for('structural_elements.edit', type=type, id=structural_element.id, tab='properties')|urlencode) %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<form id="delForm" action="{{ url_for('timeseries.delete', id=timeseries.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ timeseries.name }}&lt;/mark&gt; timeseries">
+<form id="delForm" action="{{ url_for('structural_elements.delete', type=type, id=structural_element.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ structural_element.name }}&lt;/mark&gt; {{ type }}">
     <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
     <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
 </form>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
         <div class="col">
-            <h5>Campaign</h5>
-            <p>{{ g.campaign_ctxt.name }}</p>
-        </div>
-        <div class="col">
-            <h5>Campaign scope</h5>
-            <p>{{ timeseries.campaign_scope_name }}</p>
-        </div>
-    </div>
-    <div class="row">
-        <div class="col">
             <ul class="nav nav-tabs app-tabs" role="tablist">
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'general' %} active{% endif %}" id="general-tab" data-bs-toggle="tab" data-bs-target="#general-tabcontent" type="button" role="tab" aria-controls="general-tabcontent" aria-selected="{% if tab == 'general' %}true{% else %}false{% endif %}">General</button>
                 </li>
                 <li class="nav-item" role="presentation">
-                    <button class="nav-link{% if tab == 'properties' %} active{% endif %}" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="{% if tab == 'properties' %}true{% else %}false{% endif %}">Properties <span class="badge bg-secondary">{{ properties|length }}</span></button>
+                    <button class="nav-link{% if tab == 'attributes' %} active{% endif %}" id="properties-tab" data-bs-toggle="tab" data-bs-target="#properties-tabcontent" type="button" role="tab" aria-controls="properties-tabcontent" aria-selected="{% if tab == 'attributes' %}true{% else %}false{% endif %}">Attributes <span class="badge bg-secondary">{{ properties|length }}</span></button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white mb-3">
                 <div class="tab-pane fade{% if tab == 'general' %} show active{% endif %} p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab">
                     <fieldset>
-                        <legend class="invisible d-none">Timeseries general informations</legend>
+                        <legend class="invisible d-none">{{ type|capitalize }} general information</legend>
                         <div class="mb-3">
                             <label class="form-label" for="name">Name</label>
-                            <input type="text" form="editForm" class="form-control" id="name" name="name" minlength="1" maxlength="80" value="{{ timeseries.name }}" required autofocus>
+                            <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ structural_element.name }}" minlength="1" maxlength="80" required autofocus>
+                        </div>
+                        {% if type == "site" %}
+                        <div class="row mb-3">
+                            <div class="col">
+                                <label class="form-label" for="latitude">Latitude <span class="fst-italic text-muted">[°]</span></label>
+                                <input type="number" form="editForm" class="form-control hide-arrows" id="latitude" name="latitude" min="-90" max="90" step="any" value="{{ structural_element.latitude }}">
+                            </div>
+                            <div class="col">
+                                <label class="form-label" for="longitude">Longitude <span class="fst-italic text-muted">[°]</span></label>
+                                <input type="number" form="editForm" class="form-control hide-arrows" id="longitude" name="longitude" min="-180" max="180" step="any" value="{{ structural_element.longitude }}">
+                            </div>
                         </div>
+                        {% endif %}
                         <div class="mb-3">
                             <label class="form-label" for="description">Description</label>
-                            <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ timeseries.description }}</textarea>
+                            <textarea form="editForm" class="form-control" id="description" name="description" maxlength="500" rows="3">{{ structural_element.description }}</textarea>
                         </div>
                         <div class="mb-3">
-                            <label class="form-label" for="unit_symbol">Unit symbol</label>
-                            <input type="text" form="editForm" class="form-control" id="unit_symbol" name="unit_symbol" maxlength="20" value="{{ timeseries.unit_symbol }}">
+                            <label class="form-label" for="ifc_id">IFC ID</label>
+                            <input type="text" form="editForm" class="form-control" id="ifc_id" name="ifc_id" value="{{ structural_element.ifc_id }}" maxlength="22">
                         </div>
                     </fieldset>
                 </div>
-                <div class="tab-pane fade{% if tab == 'properties' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
+                <div class="tab-pane fade{% if tab == 'attributes' %} show active{% endif %} p-3" id="properties-tabcontent" role="tabpanel" aria-labelledby="properties-tab">
                     <fieldset>
-                        <legend class="invisible d-none">Timeseries properties</legend>
+                        <legend class="invisible d-none">{{ type|capitalize }} attributes</legend>
                         {% for property_id, property_data in properties.items() %}
                         <div class="mb-3">
                             <label class="form-label" for="property-{{ property_id }}">{{ property_data.name }}{% if property_data.unit_symbol %}<span class="fst-italic text-muted ms-1">[{{ property_data.unit_symbol }}]</span>{% endif %}</label>
                             <input type="hidden" form="editForm" class="form-control" id="property-{{ property_id }}-etag" name="property-{{ property_id }}-etag" value="{{ property_data.etag }}">
                             <div class="d-flex justify-content-between align-items-top gap-3">
                                 <div class="w-100">
                                     {% if property_data.value_type == "boolean" %}
@@ -70,61 +76,61 @@
                                         <input type="checkbox"{% if property_data.value == "true" %} checked{% endif %} form="editForm" class="form-check-input" role="switch" id="property-{{ property_id }}" name="property-{{ property_id }}">
                                     </div>
                                     {% else %}
                                     <input {% if property_data.value_type == "string" %}type="text" maxlength="100"{% elif property_data.value_type in ["integer", "float"] %}type="number"{% if property_data.value_type == "float" %} step="0.01"{% endif %}{% endif %} form="editForm" class="form-control" id="property-{{ property_id }}" name="property-{{ property_id }}" value="{{ property_data.value }}" required>
                                     {% endif %}
                                     <small class="fst-italic text-muted">{{ [property_data.description, property_data.value_type] | select | join(", ") }}</small>
                                 </div>
-                                <form class="mt-1" id="delPropertyForm-{{ property_data.id }}" action="{{ url_for('timeseries.delete_property', id=timeseries.id, property_id=property_data.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property_data.name }}&lt;/mark&gt; property">
+                                <form class="mt-1" id="delPropertyForm-{{ property_data.id }}" action="{{ url_for('structural_elements.delete_property', type=type, id=structural_element.id, property_id=property_data.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property_data.name }}&lt;/mark&gt; attribute">
                                     <input type="hidden" form="delPropertyForm-{{ property_data.id }}" id="delPropertyEtag-{{ property_data.id }}" name="delPropertyEtag-{{ property_data.id }}" value="{{ property_data.etag }}">
-                                    <button type="submit" form="delPropertyForm-{{ property_data.id }}" class="btn btn-sm btn-outline-danger" title="Delete property"><i class="bi bi-trash"></i></button>
+                                    <button type="submit" form="delPropertyForm-{{ property_data.id }}" class="btn btn-sm btn-outline-danger" title="Delete attribute"><i class="bi bi-trash"></i></button>
                                 </form>
                             </div>
                         </div>
                         {% endfor %}
                         <div class="d-flex justify-content-center mb-3">
                             {% if available_properties|length > 0 %}
                             <div class="dropdown">
                                 <button class="btn btn-sm btn-outline-primary dropdown-toggle" type="button" id="addPropertyBtn" data-bs-toggle="dropdown" aria-expanded="false">
-                                    <i class="bi bi-plus-circle"></i> Define a property
+                                    <i class="bi bi-plus-circle me-1"></i>Define an attribute
                                 </button>
-                                <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
-                                    <li><a class="dropdown-item" role="button" data-bs-toggle="modal" data-bs-target="#addProperty">Choose from available properties ({{ available_properties|length }})</a></li>
-                                    <li><a class="dropdown-item" href="{{ url_create_property }}">Create a new property</a></li>
+                                <ul class="dropdown-menu" aria-labelledby="addPropertyBtn">
+                                    <li><a class="dropdown-item" role="button" data-bs-toggle="modal" data-bs-target="#addProperty">Choose from available attributes ({{ available_properties|length }})</a></li>
+                                    <li><a class="dropdown-item" href="{{ url_create_property }}">Create a new attribute</a></li>
                                 </ul>
                             </div>
                             {% else %}
-                            <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new property"><i class="bi bi-plus-circle"></i> Add a new property</a>
+                            <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new attribute"><i class="bi bi-plus-circle"></i> Add a new attribute</a>
                             {% endif %}
                         </div>
                     </fieldset>
                 </div>
             </div>
             <div class="d-flex justify-content-end gap-2">
-                <a href="{{ url_for('timeseries.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
-                <form id="editForm" action="{{ url_for('timeseries.edit', id=timeseries.id) }}" method="POST">
+                <a href="{{ url_for('structural_elements.explore') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
+                <form id="editForm" action="{{ url_for('structural_elements.edit', type=type, id=structural_element.id) }}" method="POST">
                     <input type="hidden" form="editForm" id="editEtag" name="editEtag" value="{{ etag }}">
-                    <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
+                    <button type="submit" form="editForm" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save me-1"></i>Save</button>
                 </form>
             </div>
         </div>
     </div>
 </div>
 <div class="modal fade" id="addProperty" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="addPropertyLabel" aria-hidden="true">
     <div class="modal-dialog modal-lg modal-dialog-centered">
         <div class="modal-content">
             <div class="modal-header">
-                <h5 class="modal-title" id="addPropertyLabel">Define a property</h5>
+                <h5 class="modal-title" id="addPropertyLabel">Define an attribute</h5>
                 <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
             </div>
             <div class="modal-body">
-                <form id="addPropertyForm" action="{{ url_for('timeseries.create_property', id=timeseries.id) }}" method="POST">
+                <form id="addPropertyForm" action="{{ url_for('structural_elements.create_property', type=type, id=structural_element.id) }}" method="POST">
                     <div class="mb-3">
-                        <label class="form-label" for="availableProperty">Available properties <span class="badge bg-secondary">{{ available_properties|length }}</span></label>
-                        <select form="addPropertyForm" class="form-select" id="availableProperty" name="availableProperty" aria-label="Select a property">
+                        <label class="form-label" for="availableProperty">Available attributes <span class="badge bg-secondary">{{ available_properties|length }}</span></label>
+                        <select form="addPropertyForm" class="form-select" id="availableProperty" name="availableProperty" aria-label="Select an attribute">
                             {% for property_id, property_data in available_properties.items() %}
                             <option value="{{ property_id }}" data-property-type="{{ property_data.value_type }}" data-property-description="{{ property_data.description }}"{% if loop.first %} selected{% endif %}>{{ property_data.name }}{% if property_data.unit_symbol %} [{{ property_data.unit_symbol }}]{% endif %}</option>
                             {% endfor %}
                         </select>
                     </div>
                     <div class="mb-3" id="availablePropertyInputContainer">
                         <input type="hidden" class="form-control" form="addPropertyForm" id="availablePropertyValueType" name="availablePropertyValueType">
@@ -132,18 +138,18 @@
                             <input class="form-control" form="addPropertyForm" id="availablePropertyValue" name="availablePropertyValue">
                         </div>
                         <small class="fst-italic text-muted" id="availablePropertyDescription"></small>
                     </div>
                 </form>
             </div>
             <div class="modal-footer d-flex justify-content-between">
-                <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new property"><i class="bi bi-plus-circle"></i> Add a new property</a>
+                <a class="btn btn-sm btn-outline-primary" href="{{ url_create_property }}" title="Create a new attribute"><i class="bi bi-plus-circle me-1"></i>Add a new attribute</a>
                 <div>
                     <button type="button" class="btn btn-sm btn-outline-secondary" data-bs-dismiss="modal">Cancel</button>
-                    <button type="submit" form="addPropertyForm" class="btn btn-sm btn-primary"><i class="bi bi-save"></i> Save</button>
+                    <button type="submit" form="addPropertyForm" class="btn btn-sm btn-primary"><i class="bi bi-save me-1"></i>Save</button>
                 </div>
             </div>
         </div>
     </div>
 </div>
 {% endblock main_content %}
 
@@ -155,14 +161,15 @@
     document.addEventListener("DOMContentLoaded", () => {
 
         let availablePropertySelectElmt = document.getElementById("availableProperty");
         let availablePropertyInputContainerElmt = document.getElementById("availablePropertyInputContainer");
         let availablePropertyInputElmt = document.getElementById("availablePropertyValue");
         let availablePropertyValueTypeElmt = document.getElementById("availablePropertyValueType");
         let availablePropertyDescriptionElmt = document.getElementById("availablePropertyDescription");
+        let addPropertyModalElmt = document.getElementById("addProperty");
 
         function updatePropertyDescription() {
             if (availablePropertySelectElmt.selectedIndex != -1) {
                 let selectedProperty = availablePropertySelectElmt.selectedOptions[0];
                 let propertyType = selectedProperty.getAttribute("data-property-type", "string");
 
                 availablePropertyInputElmt.removeAttribute("readonly");
@@ -194,28 +201,33 @@
                         availablePropertyInputElmt.classList.replace("form-control", "form-check-input");
                         availablePropertyInputElmt.type = "checkbox";
                         availablePropertyInputElmt.setAttribute("role", "switch");
                         availablePropertyInputElmt.parentElement.classList.add("form-check", "form-switch");
                         break;
                 }
 
+                availablePropertyInputElmt.focus();
+
                 availablePropertyDescriptionElmt.innerHTML = [selectedProperty.getAttribute("data-property-description"), propertyType].filter(Boolean).join(", ");
             }
             else {
                 availablePropertyInputElmt.setAttribute("readonly", true);
                 availablePropertyDescriptionElmt.innerHTML = "";
             }
         }
 
-        if (availablePropertySelectElmt.selectedIndex != -1) {
+        availablePropertySelectElmt.addEventListener("change", () => {
             updatePropertyDescription();
-        }
-        availablePropertySelectElmt.addEventListener("change", (event) => {
-            event.preventDefault();
+        });
 
-            updatePropertyDescription();
+        addPropertyModalElmt.addEventListener("shown.bs.modal", () => {
+            availablePropertyInputElmt.focus();
         });
 
+        if (availablePropertySelectElmt.selectedIndex != -1) {
+            updatePropertyDescription();
+        }
+
     });
 </script>
 {% endfilter %}
 {% endblock body_scripts %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/list.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,35 @@
 {% extends "pages/base.html" %}
 
 {% set title = "Timeseries" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<div class="d-lg-flex d-grid gap-3">
-    {% if signed_user.is_admin %}
-    <a href="{{ url_for('timeseries.semantic_setup') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Semantic setup"><i class="bi bi-tags"></i> Semantic setup</a>
-    <a href="{{ url_for('timeseries.manage_structural_elements') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage timeseries locations"><i class="bi bi-pin-map"></i> Manage locations</a>
-    <div class="vr d-none d-lg-block mx-2"></div>
-    {% endif %}
-    <a href="{{ url_for('timeseries.create') }}" class="btn btn-sm btn-outline-primary text-nowrap ms-auto" title="Add a new timeseries"><i class="bi bi-plus-circle"></i> New timeseries</a>
+{% if signed_user.is_admin %}
+<div class="d-none d-lg-flex gap-2">
+    <a href="{{ url_for('timeseries.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new timeseries"><i class="bi bi-plus-circle"></i> Add</a>
+    <div class="vr mx-1"></div>
+    <a href="{{ url_for('timeseries.upload') }}" class="btn btn-sm btn-outline-success text-nowrap" title="Import CSV file"><i class="bi bi-upload"></i> Import CSV</a>
+    <div class="vr mx-2"></div>
+    <a href="{{ url_for('timeseries.semantic_setup') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Set timeseries semantics"><i class="bi bi-tags"></i> Set semantics</a>
+    <a href="{{ url_for('timeseries.manage_structural_elements') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Set timeseries locations"><i class="bi bi-pin-map"></i> Set locations</a>
 </div>
+<div class="btn-group d-lg-none">
+    <button id="dropdownActions" type="button" class="btn btn-sm btn-outline-primary text-nowrap dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false" title="Manage timeseries"><i class="bi bi-three-dots-vertical"></i> Actions</button>
+    <ul class="dropdown-menu" aria-labelledby="dropdownActions">
+        <li><a class="dropdown-item" href="{{ url_for('timeseries.create') }}" title="Add a new timeseries">Add timeseries</a></li>
+        <li><a class="dropdown-item" href="{{ url_for('timeseries.upload') }}" title="Import CSV file">Import CSV</a></li>
+        <li><hr class="dropdown-divider"></li>
+        <li><a class="dropdown-item" href="{{ url_for('timeseries.semantic_setup') }}" title="Set timeseries semantics">Set semantics</a></li>
+        <li><hr class="dropdown-divider"></li>
+        <li><a class="dropdown-item" href="{{ url_for('timeseries.manage_structural_elements') }}" title="Set timeseries locations">Set locations</a></li>
+    </ul>
+</div>
+{% endif %}
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-4">
@@ -29,15 +42,15 @@
                             <span class="fw-bold text-secondary"><i class="bi bi-funnel"></i> Filters</span>
                         </button>
                     </h2>
                     <div id="collapseFilters" class="accordion-collapse collapse{% if is_filtered %} show{% endif %}" aria-labelledby="headingFilters" data-bs-parent="#accordionFilters">
                         <div class="accordion-body">
                             <div class="row mb-3">
                                 <div class="col-12 col-xl-6">
-                                    <label for="siteSelector" class="form-label">Site/building... selection</label>
+                                    <label for="siteSelector" class="form-label">Sites selection</label>
                                     {% filter indent(width=12, first=False) %}
                                     {{ mac_struct_elmt_selector.render_site_selector(html_element_id="siteSelector", title=none) -}}
                                     {% endfilter %}
                                     <input type="hidden" form="formFilters" id="structural_element_filter" name="{{ filters['structural_element_filter_type'] }}" value="{{ filters['structural_element_filter_id'] }}">
                                     <div class="form-check form-switch">
                                         <input class="form-check-input" type="checkbox" form="formFilters" role="switch" id="structural_element_recursive" name="structural_element_recursive"{% if filters["structural_element_recursive"] %} checked {% endif %}>
                                         <label class="form-check-label" for="structural_element_recursive">extend search to sub-locations</label>
@@ -127,15 +140,15 @@
                     <div id="panelCollapseTimeseries-{{ x.id }}" class="accordion-collapse collapse" aria-labelledby="panelHeadingTimeseries-{{ x.id }}" data-ts-id="{{ x.id }}">
                         <div class="accordion-body">
                             <ul class="nav nav-tabs app-tabs justify-content-center" role="tablist">
                                 <li class="nav-item" role="presentation">
                                     <button class="nav-link active" id="general-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#general-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="general-tabcontent-{{ x.id }}" aria-selected="true">General</button>
                                 </li>
                                 <li class="nav-item" role="presentation">
-                                    <button class="nav-link" id="properties-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#properties-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="properties-tabcontent-{{ x.id }}">Properties</button>
+                                    <button class="nav-link" id="attributes-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#attributes-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="attributes-tabcontent-{{ x.id }}">Attributes</button>
                                 </li>
                                 <li class="nav-item" role="presentation">
                                     <button class="nav-link" id="locations-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#locations-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="locations-tabcontent-{{ x.id }}">Locations</button>
                                 </li>
                                 <li class="nav-item" role="presentation">
                                     <button class="nav-link" id="stats-tab-{{ x.id }}" data-bs-toggle="tab" data-bs-target="#stats-tabcontent-{{ x.id }}" type="button" role="tab" aria-controls="stats-tabcontent-{{ x.id }}">Data statistics</button>
                                 </li>
@@ -148,16 +161,16 @@
                                     <div class="d-flex justify-content-between align-items-start gap-3 mb-2">
                                         <small>{{ x.description }}</small>
                                         {% if signed_user.is_admin %}
                                         <a class="btn btn-sm btn-outline-secondary text-nowrap" href="{{ url_for('timeseries.edit', id=x.id) }}" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
                                         {% endif %}
                                     </div>
                                 </div>
-                                <div class="tab-pane fade p-3" id="properties-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="properties-tab-{{ x.id }}">
-                                    <div id="timeseriesProperties-{{ x.id }}" data-ts-loaded="false"></div>
+                                <div class="tab-pane fade p-3" id="attributes-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="attributes-tab-{{ x.id }}">
+                                    <div id="timeseriesAttributes-{{ x.id }}" data-ts-loaded="false"></div>
                                 </div>
                                 <div class="tab-pane fade p-3" id="locations-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="locations-tab-{{ x.id }}">
                                     <div id="timeseriesStructuralElements-{{ x.id }}" data-ts-loaded="false"></div>
                                 </div>
                                 <div class="tab-pane fade p-3" id="stats-tabcontent-{{ x.id }}" role="tabpanel" aria-labelledby="tats-tab-{{ x.id }}">
                                     <div class="row mb-2 gap-3">
                                         <div class="col-auto">
```

#### html2text {}

```diff
@@ -1,21 +1,27 @@
 {% import "macros/components/structural_element_selector.html" as
 mac_struct_elmt_selector %} {% extends "pages/base.html" %} {% set title =
 "Timeseries" %} {% block main_toolbar %} {{ super() -}} {% filter indent
-(width=20, first=True) %}
-{% if signed_user.is_admin %}
- Semantic_setup
+(width=20, first=True) %} {% if signed_user.is_admin %}
+ Add
+ Import_CSV
+ Set_semantics
 
- Manage_locations
-{% endif %}
- New_timeseries
-{% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
--}}
+ Set_locations
+ Actions
+    * Add_timeseries
+    * Import_CSV
+    * =========================================================================
+    * Set_semantics
+    * =========================================================================
+    * Set_locations
+{% endif %} {% endfilter %} {% endblock main_toolbar %} {% block main_content
+%} {{ super() -}}
   Filters
-Site/building... selection {% filter indent(width=12, first=False) %} {
+Sites selection {% filter indent(width=12, first=False) %} {
 { mac_struct_elmt_selector.render_site_selector(html_element_id="siteSelector",
 title=none) -}} {% endfilter %}
 % if filters["structural_element_recursive"] %} checked {% endif %}> extend
 search to sub-locations
 Zone selection {% filter indent(width=12, first=False) %} {
 { mac_struct_elmt_selector.render_zone_selector(html_element_id="zoneSelector",
 title=none) -}} {% endfilter %}
@@ -53,15 +59,15 @@
 % if pagination.page != pagination.last_page %} role="button" title="Last page"
 data-page="{{ pagination.last_page }}"{% endif %}>
 {% if timeseries|length > 0 %}
 {% for x in timeseries %}
  {{ x.name }} {% if x.unit_symbol %} [{{ x.unit_symbol }}] {% endif %}
 {{ x.campaign_scope_name }}
     * General
-    * Properties
+    * Attributes
     * Locations
     * Data statistics
     * Events
 {{ x.description }} {% if signed_user.is_admin %}
  Edit
  {% endif %}
 {% for ts_datastate in ts_data_states %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 {% set subtitle = "Manage locations" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row h-100">
         <div class="col-12 col-xl-6 pb-3 pb-xl-0">
-            <h5>Timeseries</h5>
             <div class="row mb-3">
                 <div class="d-flex align-items-center gap-2">
                     <label class="form-label m-0" for="search">Search</label>
-                    <input type="text" class="form-control" id="search" name="search" autofocus>
+                    <input type="text" class="form-control form-control-sm" id="search" name="search" placeholder="Name..." data-bs-toggle="tooltip" data-bs-html="true" data-bs-title="Hit <b>enter</b> to filter timeseries" autofocus></input>
                     <a id="clear" role="button" class="link-danger text-decoration-none mx-1 d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
                 </div>
             </div>
             <nav class="row mb-2" aria-label="Timeseries pagination">
                 <div class="col-auto d-flex align-items-center py-1">
                     <div id="tsPageSizeSelectorContainer"></div>
                 </div>
@@ -28,23 +27,19 @@
             <div class="row">
                 <div class="col">
                     <div id="tsListContainer"></div>
                 </div>
             </div>
         </div>
         <div class="col">
-            <h5>
-                Locations available
-                <sup><a class="link-secondary" title="Help" role="button" data-bs-toggle="collapse" data-bs-target="#helpLocations" aria-expanded="false" aria-controls="helpLocations"><i class="bi bi-question-diamond"></i></a></sup>
-            </h5>
-            <div class="collapse mb-3" id="helpLocations">
-                <div class="alert alert-info pb-0" role="alert">
-                    <span class="fw-bold"><i class="bi bi-question-diamond"></i> Help</span>
-                    <p class="ms-3">Click on a node in sites or zones tree to <span class="fw-bold fst-italic">drag and drop it over a timeseries</span> you want to locate.</p>
-                </div>
+            <h5 class="text-secondary">Locations available</h5>
+            <div class="alert alert-info alert-dismissible fade show" role="alert">
+                <i class="bi bi-info-square float-start me-2"></i>
+                <span>Open a timeseries accordion panel to <span class="fw-bold fst-italic">drag and drop</span> locations over it.</span>
+                <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
             </div>
             <ul class="nav nav-tabs app-tabs" id="tabSites" role="tablist">
                 <li class="nav-item" role="presentation">
                     <button class="nav-link active" id="sites-tab" data-bs-toggle="tab" data-bs-target="#sites-tabcontent" type="button" role="tab" aria-controls="sites-tabcontent" aria-selected="true"><i class="bi bi-buildings"></i> Sites / Buildings...</button>
                 </li>
                 <li class="nav-item" role="presentation">
                     <button class="nav-link" id="zones-tab" data-bs-toggle="tab" data-bs-target="#zones-tabcontent" type="button" role="tab" aria-controls="zones-tabcontent" aria-selected="false"><i class="bi bi-bullseye"></i> Zones</button>
@@ -70,13 +65,13 @@
 <script type="module">
     import { TimeseriesManageStructuralElementsView } from "{{ url_for('static', filename='scripts/modules/views/timeseries/manageStructuralElements.js') }}";
 
 
     document.addEventListener("DOMContentLoaded", () => {
 
         let tsManageStructuralElementsView = new TimeseriesManageStructuralElementsView();
-        tsManageStructuralElementsView.refresh();
+        tsManageStructuralElementsView.mount();
 
 });
 </script>
 {% endfilter %}
 {% endblock body_scripts %}
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
 {% extends "pages/base.html" %} {% set title = "Timeseries" %} {% set subtitle
 = "Manage locations" %} {% block main_content %} {{ super() -}}
-** Timeseries **
 Search [search              ]
-Locations available
- Help
-Click on a node in sites or zones tree to drag and drop it over a timeseries
-you want to locate.
+** Locations available **
+ Open a timeseries accordion panel to drag and drop locations over it.
     *  Sites / Buildings...
     *  Zones
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/create.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create a new timeseries property" %}
+{% set title = "New timeseries attribute" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('timeseries.properties.create', next=url_cancel) }}" method="POST">
                 <fieldset>
-                    <legend class="invisible d-none">Timeseries property informations</legend>
-                    <div class="mb-3">
-                        <label class="form-label" for="name">Name</label>
-                        <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
+                    <legend class="invisible d-none">Timeseries attribute information</legend>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="name">Name</label>
+                            <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
+                        </div>
                     </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="value_type">Type</label>
-                        <select class="form-select" id="value_type" name="value_type" aria-label="Select a value" required>
-                            <option value="integer">integer</option>
-                            <option value="float">float</option>
-                            <option value="boolean">boolean</option>
-                            <option value="string">string</option>
-                        </select>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="value_type">Type</label>
+                            <select class="form-select" id="value_type" name="value_type" aria-label="Select a value" required>
+                                {% for x in property_value_types %}
+                                <option value="{{ x.name }}">{{ x.value }}</option>
+                                {% endfor %}
+                            </select>
+                        </div>
+                        <div class="col">
+                            <label class="form-label" for="unit_symbol">Unit symbol</label>
+                            <input type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20">
+                        </div>
                     </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="unit_symbol">Unit symbol</label>
-                        <input type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20">
-                    </div>
-                    <div class="mb-3">
-                        <label class="form-label" for="description">Description</label>
-                        <textarea class="form-control" id="description" name="description" maxlength="250" rows="3"></textarea>
+                    <div class="row mb-3">
+                        <div class="col">
+                            <label class="form-label" for="description">Description</label>
+                            <textarea class="form-control" id="description" name="description" maxlength="250" rows="3"></textarea>
+                        </div>
                     </div>
                     <div class="d-flex justify-content-end gap-2">
                         <a href="{{ url_cancel }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                         <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
                     </div>
                 </fieldset>
             </form>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-{% extends "pages/base.html" %} {% set title = "Create a new timeseries
-property" %} {% block main_content %} {{ super() -}}
- Timeseries property informations
+{% extends "pages/base.html" %} {% set title = "New timeseries attribute" %} {%
+block main_content %} {{ super() -}}
+ Timeseries attribute information
 Name [name                ]
-Type [One of: integer/float/boolean/string]
+{% for x in property_value_types %}
+{{ x.value }}
+{% endfor %}
 Unit symbol [unit_symbol         ]
 Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/edit.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Timeseries property" %}
+{% set title = "Timeseries attribute" %}
 {% set subtitle = "Edit" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<form id="delForm" action="{{ url_for('timeseries.properties.delete', id=property.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property.name }}&lt;/mark&gt; timeseries property">
+<form id="delForm" action="{{ url_for('timeseries.properties.delete', id=property.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ property.name }}&lt;/mark&gt; timeseries attribute">
     <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
     <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
 </form>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <fieldset>
-                <legend class="invisible d-none">Timeseries property informations</legend>
-                <div class="mb-3">
-                    <label class="form-label" for="name">Name</label>
-                    <input type="text" form="editForm" class="form-control" id="name" name="name" minlength="1" maxlength="80" value="{{ property.name }}" required autofocus>
+                <legend class="invisible d-none">Timeseries attribute information</legend>
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="name">Name</label>
+                        <input type="text" form="editForm" class="form-control" id="name" name="name" minlength="1" maxlength="80" value="{{ property.name }}" required autofocus>
+                    </div>
                 </div>
-                <div class="mb-3">
-                    <label class="form-label" for="value_type">Type</label>
-                    <input type="text" class="form-control" id="value_type" name="value_type" value="{{ property.value_type }}" readonly>
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="value_type">Type</label>
+                        <input type="text" class="form-control" id="value_type" name="value_type" value="{{ property.value_type }}" disabled readonly>
+                    </div>
+                    <div class="col">
+                        <label class="form-label" for="unit_symbol">Unit symbol</label>
+                        <input form="editForm" type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20" value="{{ property.unit_symbol }}">
+                    </div>
                 </div>
-                <div class="mb-3">
-                    <label class="form-label" for="unit_symbol">Unit symbol</label>
-                    <input form="editForm" type="text" class="form-control" id="unit_symbol" name="unit_symbol" minlength="1" maxlength="20" value="{{ property.unit_symbol }}">
-                </div>
-                <div class="mb-3">
-                    <label class="form-label" for="description">Description</label>
-                    <textarea form="editForm" class="form-control" id="description" name="description" maxlength="250" rows="3">{{ property.description }}</textarea>
+                <div class="row mb-3">
+                    <div class="col">
+                        <label class="form-label" for="description">Description</label>
+                        <textarea form="editForm" class="form-control" id="description" name="description" maxlength="250" rows="3">{{ property.description }}</textarea>
+                    </div>
                 </div>
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('timeseries.properties.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                     <form id="editForm" action="{{ url_for('timeseries.properties.edit', id=property.id) }}" method="POST">
                         <input type="hidden" form="editForm" id="editEtag" name="editEtag" value="{{ etag }}">
                         <button type="submit" form="editForm" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
                     </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-{% extends "pages/base.html" %} {% set title = "Timeseries property" %} {% set
+{% extends "pages/base.html" %} {% set title = "Timeseries attribute" %} {% set
 subtitle = "Edit" %} {% block main_toolbar %} {{ super() -}} {% filter indent
 (width=20, first=True) %}
   Delete
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
- Timeseries property informations
+ Timeseries attribute information
 Name [{{ property.name }} ]
 Type [{{ property.value_type }}]
 Unit symbol [{{ property.unit_symbol }}]
 Description
 {{ property.description }}
 Cancel
   Save
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/list.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Timeseries properties" %}
+{% set title = "Timeseries attributes" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('timeseries.properties.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new timeseries property"><i class="bi bi-plus-circle"></i> New property</a>
+<a href="{{ url_for('timeseries.properties.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new timeseries attribute"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
@@ -37,15 +37,15 @@
                             <td>
                                 {% if prop.description|length > 80 %}
                                 <abbr title="{{ prop.description }}">{{ prop.description | truncate(80) }}</abbr>
                                 {% else %}
                                 {{ prop.description }}
                                 {% endif %}
                             </td>
-                            <td class="text-center"><a class="btn btn-sm btn-outline-secondary" href="{{ url_for('timeseries.properties.edit', id=prop.id) }}" title="Edit property"><i class="bi bi-pencil"></i></td>
+                            <td class="text-center"><a class="btn btn-sm btn-outline-secondary" href="{{ url_for('timeseries.properties.edit', id=prop.id) }}" title="Edit attribute"><i class="bi bi-pencil"></i></td>
                         </tr>
                         {% endfor %}
                     </tbody>
                 </table>
             </div>              
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "pages/base.html" %} {% set title = "Timeseries properties" %} {%
+{% extends "pages/base.html" %} {% set title = "Timeseries attributes" %} {%
 block main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
- New_property
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
 Name            Type               Unit                Description
                                                        {% if
                                                        prop.description|length
                 {{ prop.value_type {{ prop.unit_symbol > 80 %} {
 {{ prop.name }} }}                 }}                  { prop.description |
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/semantic_setup.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/create.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/create.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% extends "pages/base.html" %}
 
-{% set title = "Create a user group" %}
+{% set title = "New group" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
         <div class="col">
             <form action="{{ url_for('user_groups.create') }}" method="POST">
                 <fieldset>
-                    <legend class="invisible d-none">User group information</legend>
+                    <legend class="invisible d-none">Group information</legend>
                     <div class="mb-3">
                         <label class="form-label" for="name">Name</label>
                         <input type="text" class="form-control" id="name" name="name" minlength="1" maxlength="80" required autofocus>
                     </div>
                     <div class="d-flex justify-content-end gap-2">
                         <a href="{{ url_for('user_groups.list') }}" class="btn btn-sm btn-outline-secondary text-break" title="Cancel">Cancel</a>
                         <button type="submit" class="btn btn-sm btn-primary text-break" title="Save"><i class="bi bi-save"></i> Save</button>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% extends "pages/base.html" %} {% set title = "Create a user group" %} {%
-block main_content %} {{ super() -}}
- User group information
+{% extends "pages/base.html" %} {% set title = "New group" %} {% block
+main_content %} {{ super() -}}
+ Group information
 Name [name                ]
 Cancel  Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/edit.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% extends "pages/base.html" %}
 
-{% set title = "User group" %}
+{% set title = "Group" %}
 {% set subtitle = "Edit" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
 {% if not self_edit %}
-<form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
+<form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; group">
     <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
     <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
 </form>
 {% endif %}
 {% endfilter %}
 {% endblock main_toolbar %}
 
@@ -23,15 +23,15 @@
             <h5>Group</h5>
             <p class="text-break">{{ user_group.name }}</p>
         </div>
     </div>
     <div class="row">
         <div class="col">
             <fieldset>
-                <legend class="invisible d-none">User group information</legend>
+                <legend class="invisible d-none">Group information</legend>
                 <div class="mb-3">
                     <label class="form-label" for="name">Name</label>
                     <input type="text" form="editForm" class="form-control" id="name" name="name" value="{{ user_group.name }}" minlength="1" maxlength="80" required autofocus>
                 </div>
                 <div class="d-flex justify-content-end gap-2">
                     <a href="{{ url_for('user_groups.view', id=user_group.id) }}" class="btn btn-outline-secondary btn-sm text-break" title="Cancel">Cancel</a>
                     <form id="editForm" action="{{ url_for('user_groups.edit', id=user_group.id) }}" method="POST">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-{% extends "pages/base.html" %} {% set title = "User group" %} {% set subtitle
-= "Edit" %} {% block main_toolbar %} {{ super() -}} {% filter indent(width=20,
+{% extends "pages/base.html" %} {% set title = "Group" %} {% set subtitle =
+"Edit" %} {% block main_toolbar %} {{ super() -}} {% filter indent(width=20,
 first=True) %} {% if not self_edit %}
   Delete
 {% endif %} {% endfilter %} {% endblock main_toolbar %} {% block main_content
 %} {{ super() -}}
 ** Group **
 {{ user_group.name }}
- User group information
+ Group information
 Name [{{ user_group.name }}]
 Cancel
   Save
 {% endblock main_content %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "pages/base.html" %}
 
-{% set title = "User group" %}
+{% set title = "Group" %}
 {% set subtitle = "Manage users" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
 <div class="d-lg-flex d-grid gap-2">
-    <a href="{{ url_for('user_groups.view', id=user_group.id) }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage user group"><i class="bi bi-arrow-return-left"></i> Back to user group</a>
+    <a href="{{ url_for('user_groups.view', id=user_group.id) }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage group"><i class="bi bi-arrow-return-left"></i> Back to group view</a>
     <div class="vr d-none d-lg-block mx-2"></div>
     <div class="hstack gap-2 ms-auto">
         {% if signed_user.is_admin %}
-        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
+        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; group">
             <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
             <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
         </form>
         {% endif %}
         <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "pages/base.html" %} {% set title = "User group" %} {% set subtitle
-= "Manage users" %} {% block main_toolbar %} {{ super() -}} {% filter indent
+{% extends "pages/base.html" %} {% set title = "Group" %} {% set subtitle =
+"Manage users" %} {% block main_toolbar %} {{ super() -}} {% filter indent
 (width=20, first=True) %}
- Back_to_user_group
+ Back_to_group_view
 {% if signed_user.is_admin %}
   Delete
 {% endif %}
  Edit
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
 ** Group **
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "pages/base.html" %}
 
-{% set title = "User group" %}
+{% set title = "Group" %}
 {% set subtitle = "Manage campaign scopes" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
 <div class="d-lg-flex d-grid gap-2">
-    <a href="{{ url_for('user_groups.view', id=user_group.id, tab='campaign_scopes') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage user group"><i class="bi bi-arrow-return-left"></i> Back to user group</a>
+    <a href="{{ url_for('user_groups.view', id=user_group.id, tab='campaign_scopes') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage group"><i class="bi bi-arrow-return-left"></i> Back to group view</a>
     <div class="vr d-none d-lg-block mx-2"></div>
     <div class="hstack gap-2 ms-auto">
         {% if signed_user.is_admin %}
-        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
+        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; group">
             <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
             <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
         </form>
         {% endif %}
         <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "pages/base.html" %} {% set title = "User group" %} {% set subtitle
-= "Manage campaign scopes" %} {% block main_toolbar %} {{ super() -}} {% filter
+{% extends "pages/base.html" %} {% set title = "Group" %} {% set subtitle =
+"Manage campaign scopes" %} {% block main_toolbar %} {{ super() -}} {% filter
 indent(width=20, first=True) %}
- Back_to_user_group
+ Back_to_group_view
 {% if signed_user.is_admin %}
   Delete
 {% endif %}
  Edit
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
   Group
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaigns.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {% extends "pages/base.html" %}
 
-{% set title = "User group" %}
+{% set title = "Group" %}
 {% set subtitle = "Manage campaigns" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
 <div class="d-lg-flex d-grid gap-2">
-    <a href="{{ url_for('user_groups.view', id=user_group.id, tab='campaigns') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage user group"><i class="bi bi-arrow-return-left"></i> Back to user group</a>
+    <a href="{{ url_for('user_groups.view', id=user_group.id, tab='campaigns') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Manage group"><i class="bi bi-arrow-return-left"></i> Back to group view</a>
     <div class="vr d-none d-lg-block mx-2"></div>
     <div class="hstack gap-2 ms-auto">
         {% if signed_user.is_admin %}
-        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
+        <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; group">
             <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
             <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
         </form>
         {% endif %}
         <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-{% extends "pages/base.html" %} {% set title = "User group" %} {% set subtitle
-= "Manage campaigns" %} {% block main_toolbar %} {{ super() -}} {% filter
-indent(width=20, first=True) %}
- Back_to_user_group
+{% extends "pages/base.html" %} {% set title = "Group" %} {% set subtitle =
+"Manage campaigns" %} {% block main_toolbar %} {{ super() -}} {% filter indent
+(width=20, first=True) %}
+ Back_to_group_view
 {% if signed_user.is_admin %}
   Delete
 {% endif %}
  Edit
 {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
 -}}
 ** Group **
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/view.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/view.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 {% extends "pages/base.html" %}
 
-{% set title = "User group" %}
+{% set title = "Group" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<div class="hstack gap-2">
-    {% if signed_user.is_admin %}
-    <form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; user group">
-        <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
-        <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
-    </form>
-    {% endif %}
-    <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
-</div>
+{% if signed_user.is_admin %}
+<form id="delForm" action="{{ url_for('user_groups.delete', id=user_group.id) }}" method="POST" data-modal-confirm-message="Delete &lt;mark&gt;{{ user_group.name }}&lt;/mark&gt; group">
+    <input type="hidden" form="delForm" id="delEtag" name="delEtag" value="{{ etag }}">
+    <button type="submit" form="delForm" class="btn btn-sm btn-outline-danger text-nowrap" title="Delete"><i class="bi bi-trash"></i> Delete</button>
+</form>
+{% endif %}
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row">
@@ -34,18 +31,25 @@
                 </li>
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'campaign_scopes' %} active{% endif %}" id="campaign-scopes-tab" data-bs-toggle="tab" data-bs-target="#campaign-scopes-tabcontent" type="button" role="tab" aria-controls="campaign-scopes-tabcontent" aria-selected="{% if tab == 'campaign_scopes' %}true{% else %}false{% endif %}">Campaign scopes <span class="badge bg-secondary">{{ campaign_scopes_count }}</span></button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white mb-3">
                 <div class="tab-pane fade{% if tab == 'general' %} show active{% endif %} p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab">
-                    <dl>
-                        <dt>Name</dt>
-                        <dd class="text-break">{{ user_group.name }}</dd>
-                    </dl>
+                    <div class="d-flex justify-content-between">
+                        <dl>
+                            <dt>Name</dt>
+                            <dd class="text-break">{{ user_group.name }}</dd>
+                        </dl>
+                        {% if signed_user.is_admin %}
+                        <div>
+                            <a href="{{ url_for('user_groups.edit', id=user_group.id) }}" class="btn btn-sm btn-outline-primary text-nowrap" role="button" title="Edit"><i class="bi bi-pencil"></i> Edit</a>
+                        </div>
+                        {% endif %}
+                    </div>
                 </div>
                 <div class="tab-pane fade{% if tab == 'users' %} show active{% endif %} p-3" id="users-tabcontent" role="tabpanel" aria-labelledby="users-tab">
                     <div class="d-lg-flex flex-nowrap d-grid justify-content-lg-between gap-3">
                         <div class="order-1 order-lg-0">
                             {% if users|length > 0 %}
                             <div class="d-flex flex-wrap mt-2 gap-2">
                                 {% for user in users %}
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-{% extends "pages/base.html" %} {% set title = "User group" %} {% block
-main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
-{% if signed_user.is_admin %}
+{% extends "pages/base.html" %} {% set title = "Group" %} {% block main_toolbar
+%} {{ super() -}} {% filter indent(width=20, first=True) %} {% if
+signed_user.is_admin %}
   Delete
-{% endif %}
- Edit
-{% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super()
--}}
+{% endif %} {% endfilter %} {% endblock main_toolbar %} {% block main_content
+%} {{ super() -}}
     * General
     * Users {{ users|length }}
     * Campaigns {{ campaigns|length }}
     * Campaign scopes {{ campaign_scopes_count }}
   Name
       {{ user_group.name }}
+{% if signed_user.is_admin %}
+ Edit
+{% endif %}
 {% if users|length > 0 %}
 {% for user in users %} {% filter indent(width=16) %} {% include "components/
 users/user_for_group.html" %} {% endfilter %} {% endfor %}
 {% else %} none {% endif %}
 {% if signed_user.is_admin %}
 Manage_users
 {% endif %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/edit.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/list.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends "pages/base.html" %}
 
 {% set title = "User accounts" %}
 
 {% block main_toolbar %}
 {{ super() -}}
 {% filter indent(width=20, first=True) %}
-<a href="{{ url_for('users.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new user"><i class="bi bi-plus-circle"></i> New user account</a>
+<a href="{{ url_for('users.create') }}" class="btn btn-sm btn-outline-primary text-nowrap" title="Add a new user"><i class="bi bi-plus-circle"></i> Add</a>
 {% endfilter %}
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %} {% set title = "User accounts" %} {% block
 main_toolbar %} {{ super() -}} {% filter indent(width=20, first=True) %}
- New_user_account
+ Add
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
   Filters
 {% for val, label in {"None": "Select a role", "True": "Only admin", "False":
 "Only NOT admin"}.items() %}
 % if val == filters["is_admin"]|string %} selected{% endif %}>{{ label }}
 {% endfor %}
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/view.html` & `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/view.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,16 @@
                     <button class="nav-link{% if tab == 'groups' %} active{% endif %}" id="groups-tab" data-bs-toggle="tab" data-bs-target="#groups-tabcontent" type="button" role="tab" aria-controls="groups-tabcontent" aria-selected="{% if tab == 'groups' %}true{% else %}false{% endif %}">Groups <span id="userGroupCount" class="badge bg-secondary">0</span></button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white">
                 <div class="tab-pane fade{% if tab == 'general' %} show active{% endif %} p-3" id="general-tabcontent" role="tabpanel" aria-labelledby="general-tab">
                     <div class="d-flex justify-content-between">
                         <dl>
-                            {% if not self_view %}
                             <dt>Name</dt>
                             <dd class="text-break">{{ user.name }}</dd>
-                            {% endif %}
                             <dt>Email address</dt>
                             <dd>{{ user.email }}</dd>
                             {% if signed_user.is_admin %}
                             <dt>Is active?</dt>
                             <dd class="d-flex gap-4">
                                 {% if user.is_active %}
                                 <span class="text-success"><i class="bi bi-hand-thumbs-up"></i> yes</span>
@@ -95,15 +93,15 @@
             </div>
         </div>
         <div class="w-100 d-lg-none d-block"></div>
         <div class="col-auto mt-lg-0 mt-3 d-none" id="userGroupAvailableColumn">
             <div class="collapse collapse-horizontal app-panel-collapse" id="userGroupAvailableCollapsePanel">
                 <div class="app-panel-collapse-body">
                     <h5>
-                        Available user groups
+                        Available groups
                         <span class="badge bg-secondary" id="userGroupAvailableCount">0</span>
                         <sup><a id="userGroupAvailableHelpLnk" class="link-secondary" title="Help" role="button" data-bs-toggle="collapse" data-bs-target="#userGroupAvailableHelpCollapsePanel" aria-expanded="false" aria-controls="userGroupAvailableHelpCollapsePanel"><i class="bi bi-question-diamond"></i></a></sup>
                     </h5>
                     <div class="collapse mb-3" id="userGroupAvailableHelpCollapsePanel">
                         <div class="alert alert-info pb-0" role="alert">
                             <span class="fw-bold"><i class="bi bi-question-diamond"></i> Help</span>
                             <p class="ms-3"><span class="fw-bold fst-italic">Drag and drop</span> in the <span class="border border-4 rounded-3 bg-white app-border-dashed text-black text-opacity-25 p-1">appropriate area</span> the groups to which the user must belong.</p>
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/__init__.py` & `bemserver-ui-0.6.0/bemserver_ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/analysis/degree_days.py` & `bemserver-ui-0.6.0/bemserver_ui/views/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/auth.py` & `bemserver-ui-0.6.0/bemserver_ui/views/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/campaign_scopes.py` & `bemserver-ui-0.6.0/bemserver_ui/views/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/campaigns.py` & `bemserver-ui-0.6.0/bemserver_ui/views/campaigns.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import bemserver_api_client.exceptions as bac_exc
 
 from bemserver_ui.extensions import auth, Roles
 from bemserver_ui.extensions.campaign_context import (
     deduce_campaign_state,
     CAMPAIGN_STATE_OVERALL,
+    CampaignState,
 )
 from bemserver_ui.extensions.timezones import get_tz_info
 from bemserver_ui.common.time import convert_html_form_datetime, convert_from_iso
 from bemserver_ui.common.exceptions import BEMServerUICommonInvalidDatetimeError
 
 
 blp = flask.Blueprint("campaigns", __name__, url_prefix="/campaigns")
@@ -37,14 +38,17 @@
             api_filters["in_name"] = ui_filters["in_name"]
     elif flask.request.method == "POST":
         ui_filters["state"] = flask.request.form["state"]
         if flask.request.form["in_name"] != "":
             ui_filters["in_name"] = flask.request.form["in_name"]
             api_filters["in_name"] = ui_filters["in_name"]
 
+    if ui_filters["state"] not in [x.name for x in CampaignState]:
+        ui_filters["state"] = CAMPAIGN_STATE_OVERALL
+
     is_filtered = ui_filters["state"] != CAMPAIGN_STATE_OVERALL or (
         ui_filters["in_name"] is not None and ui_filters["in_name"] != ""
     )
 
     # Get campaign list.
     campaigns_resp = flask.g.api_client.campaigns.getall(
         sort="+name",
@@ -196,14 +200,15 @@
         )
         flask.flash("Campaign updated!", "success")
         return flask.redirect(flask.url_for("campaigns.view", id=id))
 
     campaign_resp = flask.g.api_client.campaigns.getone(id)
 
     campaign_data = campaign_resp.data
+    campaign_data["state"] = deduce_campaign_state(campaign_data)
     campaign_tz = zoneinfo.ZoneInfo(campaign_data["timezone"])
 
     try:
         full_start_time = convert_from_iso(
             campaign_data.get("start_time"), tz=campaign_tz
         )
     except BEMServerUICommonInvalidDatetimeError:
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/events/categories.py` & `bemserver-ui-0.6.0/bemserver_ui/views/events/categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/events/events.py` & `bemserver-ui-0.6.0/bemserver_ui/views/events/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/main.py` & `bemserver-ui-0.6.0/bemserver_ui/views/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,24 @@
     app.register_blueprint(blp)
 
 
 @blp.route("/")
 @blp.route("/index")
 @auth.signin_required
 def index():
-    if flask.g.campaign_ctxt.has_campaign:
-        return flask.redirect(flask.url_for("structural_elements.explore"))
-    return flask.redirect(
-        flask.url_for("campaigns.list", state=CampaignState.ongoing.value)
-    )
+    if not flask.g.campaign_ctxt.has_campaign:
+        return flask.render_template(
+            "pages/start.html", default_campaign_state=CampaignState.ongoing.value
+        )
+    return flask.redirect(flask.url_for("structural_elements.explore"))
 
 
-@blp.route("/home")
+@blp.route("/stats")
 @auth.signin_required
-def home():
-
+def stats():
     campaign_scopes_count_overall = 0
     cs_resp = flask.g.api_client.campaign_scopes.getall()
     campaign_scopes_count_overall = len(cs_resp.data)
 
     campaign_scopes_count = 0
     if flask.g.campaign_ctxt.has_campaign:
         cs_resp = flask.g.api_client.campaign_scopes.getall(
@@ -67,15 +66,15 @@
         if flask.g.campaign_ctxt.has_campaign:
             struct_elmt_resp = api_resource.getall(
                 campaign_id=flask.g.campaign_ctxt.id,
             )
             struct_elmt_count[struct_elmt_type] = len(struct_elmt_resp.data)
 
     return flask.render_template(
-        "pages/home.html",
+        "pages/stats.html",
         campaign_scopes_count_overall=campaign_scopes_count_overall,
         campaign_scopes_count=campaign_scopes_count,
         ts_count_overall=ts_count_overall,
         ts_count=ts_count,
         structural_element_types=FULL_STRUCTURAL_ELEMENT_TYPES,
         structural_element_count_overall=struct_elmt_count_overall,
         structural_element_count=struct_elmt_count,
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/notifications.py` & `bemserver-ui-0.6.0/bemserver_ui/views/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/services/cleanup.py` & `bemserver-ui-0.6.0/bemserver_ui/views/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/services/missing_data.py` & `bemserver-ui-0.6.0/bemserver_ui/views/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/services/outlier_data.py` & `bemserver-ui-0.6.0/bemserver_ui/views/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/properties.py` & `bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/properties.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Structural element properties views"""
 from copy import deepcopy
 import urllib.parse
 import flask
 
 import bemserver_api_client.exceptions as bac_exc
+from bemserver_api_client.enums import StructuralElementPropertyValueType
 
 from bemserver_ui.extensions import auth, Roles
 from bemserver_ui.common.const import FULL_STRUCTURAL_ELEMENT_TYPES
 
 
 blp = flask.Blueprint("properties", __name__, url_prefix="/properties")
 
@@ -79,28 +80,28 @@
             "name": flask.request.form["name"],
             "value_type": flask.request.form["value_type"],
             "unit_symbol": flask.request.form["unit_symbol"],
             "description": flask.request.form["description"],
         }
         ret_resp = flask.g.api_client.structural_element_properties.create(payload)
         prop_name = ret_resp.data["name"]
-        flask.flash(f"New property created: {prop_name}", "success")
+        flask.flash(f"New attribute created: {prop_name}", "success")
 
         payload = {"structural_element_property_id": ret_resp.data["id"]}
         for x in FULL_STRUCTURAL_ELEMENT_TYPES:
             if x in flask.request.form:
                 api_resource = getattr(flask.g.api_client, f"{x}_properties")
                 try:
                     api_resource.create(payload)
                 except bac_exc.BEMServerAPIValidationError:
                     flask.flash(
-                        f"Error while adding {prop_name} property to {x}s!", "error"
+                        f"Error while adding {prop_name} attribute to {x}s!", "error"
                     )
                 else:
-                    flask.flash(f"{prop_name} property added to {x}s", "success")
+                    flask.flash(f"{prop_name} attribute added to {x}s", "success")
 
         url_next = urllib.parse.unquote(
             flask.request.args.get("next")
             or flask.url_for("structural_elements.properties.list")
         )
 
         return flask.redirect(url_next)
@@ -110,14 +111,15 @@
         or flask.url_for("structural_elements.properties.list")
     )
 
     return flask.render_template(
         "pages/structural_elements/properties/create.html",
         structural_elements=FULL_STRUCTURAL_ELEMENT_TYPES,
         url_cancel=url_cancel,
+        property_value_types=StructuralElementPropertyValueType,
     )
 
 
 @blp.route("/<int:id>/edit", methods=["GET", "POST"])
 @auth.signin_required(roles=[Roles.admin])
 def edit(id):
     if flask.request.method == "POST":
@@ -126,15 +128,15 @@
             "unit_symbol": flask.request.form["unit_symbol"],
             "description": flask.request.form["description"],
         }
         prop_resp = flask.g.api_client.structural_element_properties.update(
             id, payload, etag=flask.request.form["editEtag"]
         )
         prop_name = prop_resp.data["name"]
-        flask.flash(f"{prop_name} property updated!", "success")
+        flask.flash(f"{prop_name} attribute updated!", "success")
 
         payload = {"structural_element_property_id": prop_resp.data["id"]}
         for x in FULL_STRUCTURAL_ELEMENT_TYPES:
             api_resource = getattr(flask.g.api_client, f"{x}_properties")
             x_props = api_resource.getall(structural_element_property_id=id)
             # Property is requested to be associated to structural element.
             # Is property already attach to structural element?
@@ -142,33 +144,33 @@
             # 2. No, create association.
             if x in flask.request.form:
                 if len(x_props.data) <= 0:
                     try:
                         api_resource.create(payload)
                     except bac_exc.BEMServerAPIValidationError:
                         flask.flash(
-                            f"Error while adding {prop_name} property to {x}s!",
+                            f"Error while adding {prop_name} attribute to {x}s!",
                             "error",
                         )
                     else:
-                        flask.flash(f"{prop_name} property added to {x}s", "success")
+                        flask.flash(f"{prop_name} attribute added to {x}s", "success")
             # Property is NOT requested to be associated.
             # Is property currently attach to structural element?
             # 1. Yes, remove association.
             # 2. No, nothing to do.
             elif len(x_props.data) == 1:
                 try:
                     api_resource.delete(x_props.data[0]["id"])
                 except bac_exc.BEMServerAPINotFoundError:
                     flask.flash(
-                        f"{prop_name} property is already removed for {x}s!",
+                        f"{prop_name} attribute is already removed for {x}s!",
                         "warning",
                     )
                 else:
-                    flask.flash(f"{prop_name} property removed from {x}s", "success")
+                    flask.flash(f"{prop_name} attribute removed from {x}s", "success")
 
         return flask.redirect(flask.url_for("structural_elements.properties.list"))
 
     prop_resp = flask.g.api_client.structural_element_properties.getone(id)
     prop_data = prop_resp.data
     extend_props_data([prop_data])
 
@@ -182,9 +184,9 @@
 
 @blp.route("/<int:id>/delete", methods=["POST"])
 @auth.signin_required(roles=[Roles.admin])
 def delete(id):
     flask.g.api_client.structural_element_properties.delete(
         id, etag=flask.request.form["delEtag"]
     )
-    flask.flash("Property deleted!", "success")
+    flask.flash("Attribute deleted!", "success")
     return flask.redirect(flask.url_for("structural_elements.properties.list"))
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/structural_elements.py` & `bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/structural_elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Structural elements views"""
 import flask
 
 import bemserver_api_client.exceptions as bac_exc
 
 from bemserver_ui.extensions import auth, Roles, ensure_campaign_context
-from bemserver_ui.common.const import FULL_STRUCTURAL_ELEMENT_TYPES
+from bemserver_ui.common.const import (
+    STRUCTURAL_ELEMENT_TYPES,
+    FULL_STRUCTURAL_ELEMENT_TYPES,
+)
+from bemserver_ui.common.tree import _get_node_level_from_type
+from bemserver_ui.internal_api.structural_elements import _build_tree_sites
 
 
 blp = flask.Blueprint(
     "structural_elements", __name__, url_prefix="/structural_elements"
 )
 
 
@@ -20,26 +25,28 @@
     return flask.render_template("pages/structural_elements/explore.html", tab=tab)
 
 
 @blp.route("/<string:type>/create", methods=["GET", "POST"])
 @auth.signin_required(roles=[Roles.admin])
 @ensure_campaign_context
 def create(type):
+    campaign_id = flask.g.campaign_ctxt.id
+
     if flask.request.method == "POST":
         payload = {
             "name": flask.request.form["name"],
             "description": flask.request.form["description"],
             "ifc_id": flask.request.form["ifc_id"],
         }
 
         if type in ("site", "zone"):
             if type == "site":
                 payload["latitude"] = flask.request.form["latitude"]
                 payload["longitude"] = flask.request.form["longitude"]
-            payload["campaign_id"] = flask.g.campaign_ctxt.id
+            payload["campaign_id"] = campaign_id
         elif type == "building":
             payload["site_id"] = flask.request.form["site"]
         elif type == "storey":
             payload["building_id"] = flask.request.form["building"]
         elif type == "space":
             payload["storey_id"] = flask.request.form["storey"]
 
@@ -52,28 +59,36 @@
                 type=type,
                 id=ret_resp.data["id"],
                 tab="properties",
             )
         )
 
     # Get parent type and list.
+    type_level = _get_node_level_from_type(type)
     parent_type = None
+    if type_level > 0:
+        parent_type = STRUCTURAL_ELEMENT_TYPES[type_level - 1]
+
+    # Load all parent structural elements tree (to get their path).
+    tree_sites = _build_tree_sites(
+        campaign_id, structural_element_types=STRUCTURAL_ELEMENT_TYPES[:type_level]
+    )
+
+    def _filter_children(nodes, node_level):
+        filtered_nodes = []
+        for node in nodes:
+            if node["node_level"] < node_level:
+                filtered_nodes.extend(_filter_children(node["nodes"], node_level))
+            elif node["node_level"] == node_level:
+                filtered_nodes.append(node)
+        return filtered_nodes
+
     parents = []
-    if type not in ("site", "zone"):
-        if type == "building":
-            parent_type = "site"
-        elif type == "storey":
-            parent_type = "building"
-        elif type == "space":
-            parent_type = "storey"
-        parents = (
-            getattr(flask.g.api_client, f"{parent_type}s")
-            .getall(campaign_id=flask.g.campaign_ctxt.id, sort="+name")
-            .data
-        )
+    if type_level > 0:
+        parents = _filter_children(tree_sites, type_level - 1)
 
     return flask.render_template(
         "pages/structural_elements/create.html",
         type=type,
         parent_type=parent_type,
         parents=parents,
     )
@@ -114,17 +129,18 @@
         ret_resp = api_resource.getone(id)
 
     elif flask.request.method == "POST":
         payload = {
             "name": flask.request.form["name"],
             "description": flask.request.form["description"],
             "ifc_id": flask.request.form["ifc_id"],
-            "latitude": flask.request.form["latitude"],
-            "longitude": flask.request.form["longitude"],
         }
+        if type == "site":
+            payload["latitude"] = flask.request.form["latitude"]
+            payload["longitude"] = flask.request.form["longitude"]
 
         ret_resp = api_resource.update(id, payload, etag=flask.request.form["editEtag"])
         flask.flash(f"{type} updated: {ret_resp.data['name']}", "success")
 
         # Update property values, only if value has changed.
         for prop_id, prop_data in properties.items():
             # Flask form is special with checkboxes, it sets:
@@ -148,18 +164,18 @@
                 api_propdata_resource.update(
                     prop_data["id"],
                     payload,
                     etag=flask.request.form[f"property-{prop_id}-etag"],
                 )
             except bac_exc.BEMServerAPIValidationError:
                 flask.flash(
-                    f"Error while setting {prop_data['name']} property!", "warning"
+                    f"Error while setting {prop_data['name']} attribute!", "warning"
                 )
             else:
-                flask.flash(f"{prop_data['name']} property updated!", "success")
+                flask.flash(f"{prop_data['name']} attribute updated!", "success")
 
         return flask.redirect(flask.url_for("structural_elements.explore"))
 
     return flask.render_template(
         "pages/structural_elements/edit.html",
         type=type,
         structural_element=ret_resp.data,
@@ -195,15 +211,15 @@
     payload = {
         f"{type}_id": id,
         f"{type}_property_id": flask.request.form["availableProperty"],
         "value": prop_value,
     }
     api_resource = getattr(flask.g.api_client, f"{type}_property_data")
     api_resource.create(payload)
-    flask.flash("Property defined!", "success")
+    flask.flash("Attribute defined!", "success")
 
     return flask.redirect(
         flask.url_for("structural_elements.edit", type=type, id=id, tab="properties")
     )
 
 
 @blp.route(
@@ -212,15 +228,15 @@
 @auth.signin_required(roles=[Roles.admin])
 @ensure_campaign_context
 def delete_property(type, id, property_id):
     api_resource = getattr(flask.g.api_client, f"{type}_property_data")
     api_resource.delete(
         property_id, etag=flask.request.form[f"delPropertyEtag-{property_id}"]
     )
-    flask.flash("Property deleted!", "success")
+    flask.flash("Attribute deleted!", "success")
     return flask.redirect(
         flask.url_for("structural_elements.edit", id=id, type=type, tab="properties")
     )
 
 
 @blp.route("/upload", methods=["GET", "POST"])
 @auth.signin_required(roles=[Roles.admin])
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/data.py` & `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/datastates.py` & `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/datastates.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/properties.py` & `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Timeseries properties views"""
 import urllib.parse
 import flask
 
+from bemserver_api_client.enums import StructuralElementPropertyValueType
+
 from bemserver_ui.extensions import auth, Roles
 
 
 blp = flask.Blueprint("properties", __name__, url_prefix="/properties")
 
 
 @blp.route("/", methods=["GET", "POST"])
@@ -25,27 +27,29 @@
             "name": flask.request.form["name"],
             "value_type": flask.request.form["value_type"],
             "unit_symbol": flask.request.form["unit_symbol"],
             "description": flask.request.form["description"],
         }
         ts_prop_resp = flask.g.api_client.timeseries_properties.create(payload)
         prop_name = ts_prop_resp.data["name"]
-        flask.flash(f"New timeseries property created: {prop_name}", "success")
+        flask.flash(f"New timeseries attribute created: {prop_name}", "success")
         url_next = urllib.parse.unquote(
             flask.request.args.get("next")
             or flask.url_for("timeseries_properties.list")
         )
         return flask.redirect(url_next)
 
     url_cancel = urllib.parse.unquote(
         flask.request.args.get("back") or flask.url_for("timeseries.properties.list")
     )
 
     return flask.render_template(
-        "pages/timeseries/properties/create.html", url_cancel=url_cancel
+        "pages/timeseries/properties/create.html",
+        url_cancel=url_cancel,
+        property_value_types=StructuralElementPropertyValueType,
     )
 
 
 @blp.route("/<int:id>/edit", methods=["GET", "POST"])
 @auth.signin_required(roles=[Roles.admin])
 def edit(id):
     if flask.request.method == "POST":
@@ -54,15 +58,15 @@
             "unit_symbol": flask.request.form["unit_symbol"],
             "description": flask.request.form["description"],
         }
         prop_resp = flask.g.api_client.timeseries_properties.update(
             id, payload, etag=flask.request.form["editEtag"]
         )
         prop_name = prop_resp.data["name"]
-        flask.flash(f"{prop_name} timeseries property updated!", "success")
+        flask.flash(f"{prop_name} timeseries attribute updated!", "success")
         return flask.redirect(flask.url_for("timeseries.properties.list"))
 
     ts_properties_resp = flask.g.api_client.timeseries_properties.getone(id)
 
     return flask.render_template(
         "pages/timeseries/properties/edit.html",
         property=ts_properties_resp.data,
@@ -72,9 +76,9 @@
 
 @blp.route("/<int:id>/delete", methods=["POST"])
 @auth.signin_required(roles=[Roles.admin])
 def delete(id):
     flask.g.api_client.timeseries_properties.delete(
         id, etag=flask.request.form["delEtag"]
     )
-    flask.flash("Timeseries property deleted!", "success")
+    flask.flash("Timeseries attribute deleted!", "success")
     return flask.redirect(flask.url_for("timeseries.properties.list"))
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/timeseries.py` & `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             if payload["value"] == prop_data["value"]:
                 continue
             flask.g.api_client.timeseries_property_data.update(
                 prop_data["id"],
                 payload,
                 etag=flask.request.form[f"property-{prop_id}-etag"],
             )
-            flask.flash(f"{prop_data['name']} property updated!", "success")
+            flask.flash(f"{prop_data['name']} attribute updated!", "success")
 
         return flask.redirect(flask.url_for("timeseries.list"))
 
     timeseries_resp = flask.g.api_client.timeseries.getone(id)
 
     campaign_scopes_resp = flask.g.api_client.campaign_scopes.getone(
         timeseries_resp.data["campaign_scope_id"]
@@ -272,27 +272,27 @@
         prop_value = "true" if prop_value == "on" else "false"
     payload = {
         "timeseries_id": id,
         "property_id": flask.request.form["availableProperty"],
         "value": prop_value,
     }
     flask.g.api_client.timeseries_property_data.create(payload)
-    flask.flash("Property value defined!", "success")
+    flask.flash("Attribute value defined!", "success")
 
     return flask.redirect(flask.url_for("timeseries.edit", id=id, tab="properties"))
 
 
 @blp.route("/<int:id>/property/<int:property_id>/delete", methods=["POST"])
 @auth.signin_required(roles=[Roles.admin])
 @ensure_campaign_context
 def delete_property(id, property_id):
     flask.g.api_client.timeseries_property_data.delete(
         property_id, etag=flask.request.form[f"delPropertyEtag-{property_id}"]
     )
-    flask.flash("Property value deleted!", "success")
+    flask.flash("Attribute value deleted!", "success")
     return flask.redirect(flask.url_for("timeseries.edit", id=id, tab="properties"))
 
 
 @blp.route("/manage_structural_elements")
 @auth.signin_required(roles=[Roles.admin])
 @ensure_campaign_context
 def manage_structural_elements():
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/user_groups.py` & `bemserver-ui-0.6.0/bemserver_ui/views/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui/views/users.py` & `bemserver-ui-0.6.0/bemserver_ui/views/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/bemserver_ui.egg-info/PKG-INFO` & `bemserver-ui-0.6.0/bemserver_ui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.3
+Version: 0.6.0
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,16 @@
         Is API published through SSL?
     **BEMSERVER_API_AUTH_METHOD = "http_basic"**
         API authentication method
     **BEMSERVER_UI_TIMEZONE_NAME = "UTC"**
         Default application timezone name, when not overrided campaign timezone
     **BEMSERVER_UI_NOTIFICATION_UPDATER_DELAY = 60000**
         Delay, in seconds, between each check of new notifications
+    **BEMSERVER_UI_USER_GUIDE_URL = https://bemserver-docs.readthedocs.io/en/latest/user_guide.html**
+        User guide URL
     *(optional)* **BEMSERVER_UI_PARTNERS_FILE = None**
         Absolute path of json file that describes the project's partners
 
         Example of ``BEMSERVER_UI_PARTNERS_FILE`` file structure::
 
             [
                 {
```

### Comparing `bemserver-ui-0.5.3/bemserver_ui.egg-info/SOURCES.txt` & `bemserver-ui-0.6.0/bemserver_ui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 bemserver_ui/static/scripts/modules/tools/parser.js
 bemserver_ui/static/scripts/modules/tools/time.js
 bemserver_ui/static/scripts/modules/tools/uuid.js
 bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
 bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
 bemserver_ui/static/scripts/modules/views/analysis/weather.js
 bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-bemserver_ui/static/scripts/modules/views/campaigns/selector.js
 bemserver_ui/static/scripts/modules/views/events/edit.js
 bemserver_ui/static/scripts/modules/views/events/list.js
 bemserver_ui/static/scripts/modules/views/notifications/explore.js
 bemserver_ui/static/scripts/modules/views/notifications/setup.js
 bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
 bemserver_ui/static/scripts/modules/views/services/missingData/list.js
 bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
@@ -121,15 +120,14 @@
 bemserver_ui/static/scripts/modules/views/users/manageGroups.js
 bemserver_ui/static/styles/app.css
 bemserver_ui/static/styles/dragndrop.css
 bemserver_ui/static/styles/main.css
 bemserver_ui/static/styles/signin.css
 bemserver_ui/static/styles/tree.css
 bemserver_ui/templates/components/header.html
-bemserver_ui/templates/components/campaigns/selector.html
 bemserver_ui/templates/components/sidebar/sidebar.html
 bemserver_ui/templates/components/sidebar/sidebar_admin.html
 bemserver_ui/templates/components/sidebar/sidebar_analysis.html
 bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
 bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
 bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
 bemserver_ui/templates/components/sidebar/sidebar_services.html
@@ -137,22 +135,24 @@
 bemserver_ui/templates/components/user_groups/group_for_campaign.html
 bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
 bemserver_ui/templates/components/user_groups/user_group_available.html
 bemserver_ui/templates/components/users/user_available.html
 bemserver_ui/templates/components/users/user_for_group.html
 bemserver_ui/templates/macros/flash.html
 bemserver_ui/templates/macros/partners.html
+bemserver_ui/templates/macros/components/campaign.html
 bemserver_ui/templates/macros/components/sidebar.html
 bemserver_ui/templates/macros/components/structural_element_selector.html
 bemserver_ui/templates/macros/components/ts_selector.html
 bemserver_ui/templates/pages/about.html
 bemserver_ui/templates/pages/base.html
-bemserver_ui/templates/pages/home.html
 bemserver_ui/templates/pages/signin.html
 bemserver_ui/templates/pages/skeleton.html
+bemserver_ui/templates/pages/start.html
+bemserver_ui/templates/pages/stats.html
 bemserver_ui/templates/pages/analysis/degree_days.html
 bemserver_ui/templates/pages/analysis/energy_consumption.html
 bemserver_ui/templates/pages/analysis/weather.html
 bemserver_ui/templates/pages/campaign_scopes/create.html
 bemserver_ui/templates/pages/campaign_scopes/edit.html
 bemserver_ui/templates/pages/campaign_scopes/list.html
 bemserver_ui/templates/pages/campaign_scopes/view.html
```

### Comparing `bemserver-ui-0.5.3/requirements/dev.txt` & `bemserver-ui-0.6.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.3/requirements/install.txt` & `bemserver-ui-0.6.0/requirements/install.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/install.txt --resolver=backtracking setup.py
 #
-bemserver-api-client==0.20.0
+bemserver-api-client==0.20.1
     # via bemserver-ui (setup.py)
 certifi==2021.10.8
     # via requests
 charset-normalizer==2.0.12
     # via requests
 click==8.1.3
     # via flask
```

### Comparing `bemserver-ui-0.5.3/setup.py` & `bemserver-ui-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="bemserver-ui",
-    version="0.5.3",
+    version="0.6.0",
     description="BEMServer web interface",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/BEMServer/bemserver-ui",
     author="NOBATEK/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
@@ -44,13 +44,13 @@
             "GNU Affero General Public License v3 or later (AGPLv3+)"
         ),
     ],
     python_requires=">=3.9",
     install_requires=[
         "flask>=2.2.3,<3.0.0",
         "python-dotenv>=1.0.0,<2.0.0",
-        "bemserver-api-client>=0.20.0,<0.21.0",
+        "bemserver-api-client>=0.20.1,<0.21.0",
     ],
     extras_require=EXTRAS_REQUIRE,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
 )
```

