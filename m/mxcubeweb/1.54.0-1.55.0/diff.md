# Comparing `tmp/mxcubeweb-1.54.0.tar.gz` & `tmp/mxcubeweb-1.55.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcubeweb-1.54.0.tar", max compression
+gzip compressed data, was "mxcubeweb-1.55.0.tar", max compression
```

## Comparing `mxcubeweb-1.54.0.tar` & `mxcubeweb-1.55.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     7652 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/LICENSE
--rw-r--r--   0        0        0     3638 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/README.md
--rw-r--r--   0        0        0     3688 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/__init__.py
--rw-r--r--   0        0        0    18662 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/app.py
--rw-r--r--   0        0        0     1409 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/config.py
--rw-r--r--   0        0        0        0 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/actuator_adapter.py
--rw-r--r--   0        0        0    13582 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/adapter_base.py
--rw-r--r--   0        0        0     1846 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/beam_adapter.py
--rw-r--r--   0        0        0     1642 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/beamline_action_adapter.py
--rw-r--r--   0        0        0     3063 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/beamline_adapter.py
--rw-r--r--   0        0        0     1586 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/data_publisher_adapter.py
--rw-r--r--   0        0        0      494 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/detector_adapter.py
--rw-r--r--   0        0        0      988 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/diffractometer_adapter.py
--rw-r--r--   0        0        0      591 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/energy_adapter.py
--rw-r--r--   0        0        0     1384 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/flux_adapter.py
--rw-r--r--   0        0        0     1992 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/machine_info_adapter.py
--rw-r--r--   0        0        0     2218 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/motor_adapter.py
--rw-r--r--   0        0        0     1763 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/nstate_adapter.py
--rw-r--r--   0        0        0     2905 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/adapter/wavelength_adapter.py
--rw-r--r--   0        0        0    12293 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/components/beamline.py
--rw-r--r--   0        0        0     1384 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/components/chat.py
--rw-r--r--   0        0        0      630 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/components/component_base.py
--rw-r--r--   0        0        0     1246 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/components/gphl_workflow.py
--rw-r--r--   0        0        0    16902 2023-06-29 14:55:12.337425 mxcubeweb-1.54.0/mxcube3/core/components/lims.py
--rw-r--r--   0        0        0    90191 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/queue.py
--rw-r--r--   0        0        0    18591 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/samplechanger.py
--rw-r--r--   0        0        0    22573 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/sampleview.py
--rw-r--r--   0        0        0     1896 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/user/database.py
--rw-r--r--   0        0        0      418 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/user/dummyusermanager.py
--rw-r--r--   0        0        0    15144 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/user/usermanager.py
--rw-r--r--   0        0        0     1986 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/components/workflow.py
--rw-r--r--   0        0        0     2344 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/models/adaptermodels.py
--rw-r--r--   0        0        0     3070 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/models/configmodels.py
--rw-r--r--   0        0        0      254 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/models/generic.py
--rw-r--r--   0        0        0     3359 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/models/usermodels.py
--rw-r--r--   0        0        0     2344 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/util/adapterutils.py
--rw-r--r--   0        0        0     1630 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/util/convertutils.py
--rw-r--r--   0        0        0      523 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/util/fsutils.py
--rw-r--r--   0        0        0     4647 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/core/util/networkutils.py
--rw-r--r--   0        0        0     1188 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/logging_handler.py
--rw-r--r--   0        0        0        0 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/__init__.py
--rw-r--r--   0        0        0     8128 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/beamline.py
--rw-r--r--   0        0        0      859 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/detector.py
--rw-r--r--   0        0        0     4033 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/diffractometer.py
--rw-r--r--   0        0        0      587 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/gphl_workflow.py
--rw-r--r--   0        0        0     5165 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/lims.py
--rw-r--r--   0        0        0     1223 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/log.py
--rw-r--r--   0        0        0     3307 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/login.py
--rw-r--r--   0        0        0     2471 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/main.py
--rw-r--r--   0        0        0     4291 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/mockups.py
--rw-r--r--   0        0        0    10369 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/queue.py
--rw-r--r--   0        0        0     6224 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/ra.py
--rw-r--r--   0        0        0    13766 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/samplecentring.py
--rw-r--r--   0        0        0     4671 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/samplechanger.py
--rw-r--r--   0        0        0    20592 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/signals.py
--rw-r--r--   0        0        0     1125 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/routes/workflow.py
--rw-r--r--   0        0        0     7438 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/server.py
--rw-r--r--   0        0        0     1396 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/state_storage.py
--rw-r--r--   0        0        0      771 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/templates/characterisation-results.js
--rw-r--r--   0        0        0     3610 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/templates/data-collection-results.html
--rw-r--r--   0        0        0   329138 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/templates/precompiled.templates.min.js
--rw-r--r--   0        0        0      721 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/templates/workflow-results.js
--rw-r--r--   0        0        0       22 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/version.py
--rw-r--r--   0        0        0        0 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/video/__init__.py
--rw-r--r--   0        0        0     2647 2023-06-29 14:55:12.341425 mxcubeweb-1.54.0/mxcube3/video/websocket-relay.js
--rw-r--r--   0        0        0     1785 2023-06-29 14:55:28.097306 mxcubeweb-1.54.0/pyproject.toml
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.54.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-07-05 06:37:12.239280 mxcubeweb-1.55.0/LICENSE
+-rw-r--r--   0        0        0     3638 2023-07-05 06:37:12.239280 mxcubeweb-1.55.0/README.md
+-rw-r--r--   0        0        0     3688 2023-07-05 06:37:12.239280 mxcubeweb-1.55.0/mxcube3/__init__.py
+-rw-r--r--   0        0        0    18662 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/app.py
+-rw-r--r--   0        0        0     1409 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/config.py
+-rw-r--r--   0        0        0        0 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2408 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/actuator_adapter.py
+-rw-r--r--   0        0        0    13582 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/adapter_base.py
+-rw-r--r--   0        0        0     1846 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/beam_adapter.py
+-rw-r--r--   0        0        0     1642 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/beamline_action_adapter.py
+-rw-r--r--   0        0        0     3063 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/beamline_adapter.py
+-rw-r--r--   0        0        0     1586 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/data_publisher_adapter.py
+-rw-r--r--   0        0        0      494 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/detector_adapter.py
+-rw-r--r--   0        0        0      988 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/diffractometer_adapter.py
+-rw-r--r--   0        0        0      591 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/energy_adapter.py
+-rw-r--r--   0        0        0     1384 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/flux_adapter.py
+-rw-r--r--   0        0        0     1992 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/machine_info_adapter.py
+-rw-r--r--   0        0        0     2218 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/motor_adapter.py
+-rw-r--r--   0        0        0     1763 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/nstate_adapter.py
+-rw-r--r--   0        0        0     2905 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/adapter/wavelength_adapter.py
+-rw-r--r--   0        0        0    12293 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/beamline.py
+-rw-r--r--   0        0        0     1384 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/chat.py
+-rw-r--r--   0        0        0      630 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/component_base.py
+-rw-r--r--   0        0        0     1246 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/gphl_workflow.py
+-rw-r--r--   0        0        0    16902 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/lims.py
+-rw-r--r--   0        0        0    90398 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/queue.py
+-rw-r--r--   0        0        0    19329 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/samplechanger.py
+-rw-r--r--   0        0        0    22573 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/sampleview.py
+-rw-r--r--   0        0        0     1896 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/user/database.py
+-rw-r--r--   0        0        0      418 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/user/dummyusermanager.py
+-rw-r--r--   0        0        0    15144 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/user/usermanager.py
+-rw-r--r--   0        0        0     1986 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/components/workflow.py
+-rw-r--r--   0        0        0     2344 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/models/adaptermodels.py
+-rw-r--r--   0        0        0     3070 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/models/configmodels.py
+-rw-r--r--   0        0        0      254 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/models/generic.py
+-rw-r--r--   0        0        0     3359 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/models/usermodels.py
+-rw-r--r--   0        0        0     2344 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/util/adapterutils.py
+-rw-r--r--   0        0        0     1630 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/util/convertutils.py
+-rw-r--r--   0        0        0      523 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/util/fsutils.py
+-rw-r--r--   0        0        0     4647 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/core/util/networkutils.py
+-rw-r--r--   0        0        0     1188 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/logging_handler.py
+-rw-r--r--   0        0        0        0 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/__init__.py
+-rw-r--r--   0        0        0     8128 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/beamline.py
+-rw-r--r--   0        0        0      859 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/detector.py
+-rw-r--r--   0        0        0     4033 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/diffractometer.py
+-rw-r--r--   0        0        0      587 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/gphl_workflow.py
+-rw-r--r--   0        0        0     5165 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/lims.py
+-rw-r--r--   0        0        0     1223 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/log.py
+-rw-r--r--   0        0        0     3307 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/login.py
+-rw-r--r--   0        0        0     2471 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/main.py
+-rw-r--r--   0        0        0     4291 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/mockups.py
+-rw-r--r--   0        0        0    10369 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/queue.py
+-rw-r--r--   0        0        0     6224 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/ra.py
+-rw-r--r--   0        0        0    13766 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/samplecentring.py
+-rw-r--r--   0        0        0     4851 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/samplechanger.py
+-rw-r--r--   0        0        0    20592 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/signals.py
+-rw-r--r--   0        0        0     1125 2023-07-05 06:37:12.243280 mxcubeweb-1.55.0/mxcube3/routes/workflow.py
+-rw-r--r--   0        0        0     7438 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/server.py
+-rw-r--r--   0        0        0     1396 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/state_storage.py
+-rw-r--r--   0        0        0      771 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/templates/characterisation-results.js
+-rw-r--r--   0        0        0     3610 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/templates/data-collection-results.html
+-rw-r--r--   0        0        0   329138 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/templates/precompiled.templates.min.js
+-rw-r--r--   0        0        0      721 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/templates/workflow-results.js
+-rw-r--r--   0        0        0       22 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/version.py
+-rw-r--r--   0        0        0        0 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/video/__init__.py
+-rw-r--r--   0        0        0     2647 2023-07-05 06:37:12.247280 mxcubeweb-1.55.0/mxcube3/video/websocket-relay.js
+-rw-r--r--   0        0        0     1785 2023-07-05 06:37:30.431815 mxcubeweb-1.55.0/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.55.0/PKG-INFO
```

### Comparing `mxcubeweb-1.54.0/LICENSE` & `mxcubeweb-1.55.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/README.md` & `mxcubeweb-1.55.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/__init__.py` & `mxcubeweb-1.55.0/mxcube3/__init__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/app.py` & `mxcubeweb-1.55.0/mxcube3/app.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/config.py` & `mxcubeweb-1.55.0/mxcube3/config.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/actuator_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/actuator_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/adapter_base.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/beam_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/beam_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/beamline_action_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/beamline_action_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/beamline_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/beamline_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/data_publisher_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/data_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/diffractometer_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/diffractometer_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/energy_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/energy_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/flux_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/flux_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/machine_info_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/machine_info_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/motor_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/motor_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/nstate_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/nstate_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/adapter/wavelength_adapter.py` & `mxcubeweb-1.55.0/mxcube3/core/adapter/wavelength_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/beamline.py` & `mxcubeweb-1.55.0/mxcube3/core/components/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/chat.py` & `mxcubeweb-1.55.0/mxcube3/core/components/chat.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/component_base.py` & `mxcubeweb-1.55.0/mxcube3/core/components/component_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/gphl_workflow.py` & `mxcubeweb-1.55.0/mxcube3/core/components/gphl_workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/lims.py` & `mxcubeweb-1.55.0/mxcube3/core/components/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/queue.py` & `mxcubeweb-1.55.0/mxcube3/core/components/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1018,14 +1018,17 @@
         sample_model.loc_str = sample_id
         sample_model.free_pin_mode = item["location"] == "Manual"
         sample_model.set_name(item["sampleName"])
         sample_model.name = item["sampleName"]
 
         if sample_model.free_pin_mode:
             sample_model.location = (None, sample_id)
+        elif HWR.beamline.diffractometer.in_plate_mode():
+            component =  HWR.beamline.sample_changer._resolve_component(item["location"])
+            sample_model.location = component.get_coords()
         else:
             sample_model.location = tuple(map(int, item["location"].split(":")))
 
         # Manually added sample, make sure that i'ts on the server side sample list
         if item["location"] == "Manual":
             item["defaultSubDir"] = self.app.lims.get_default_subdir(item)
             self.app.lims.sample_list_update_sample(sample_id, item)
```

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/samplechanger.py` & `mxcubeweb-1.55.0/mxcube3/core/components/samplechanger.py`

 * *Files 12% similar despite different names*

```diff
@@ -229,15 +229,16 @@
             # Clean up if the new sample was mounted or the current sample was
             # unmounted and the new one, for some reason, failed to mount
             if res or (not res and not sc.get_loaded_sample()):
                 HWR.beamline.sample_view.clear_all()
 
                 # We remove the current sample from the queue, if we are moving
                 # from one sample to another and the current sample is in the queue
-                if sid and current_queue[sid]:
+
+                if sid and current_queue.get(sid, False):
                     node_id = current_queue[sid]["queueID"]
                     self.app.queue.set_enabled_entry(node_id, False)
                     signals.queue_toggle_sample(self.app.queue.get_entry(node_id)[1])
         finally:
             signals.sc_load_ready(sample["location"])
 
         return res
@@ -346,14 +347,42 @@
             "cmds": {"cmds": cmds},
             "msg": msg,
             "plate_mode": HWR.beamline.diffractometer.in_plate_mode(),
         }
 
         return initial_state
 
+    def sync_with_crims(self):
+        """
+        To be use mostly when Diffractometer is in plate mode
+        This retun a List of crystal dict available in Crims that have been Harvested  
+        With this user can visualize easier where the crystal are in Plate GUI  
+        """
+        xtal_list = []
+        try:
+            processing_plan = HWR.beamline.sample_changer.sync_with_crims()
+            for x in processing_plan.plate.xtal_list:
+                response = {
+                    "crystal_uuid": x.crystal_uuid,
+                    "row": x.row,
+                    "column": x.column,
+                    "shelf": x.shelf,
+                    "offset_x": x.offset_x,
+                    "offset_y": x.offset_y,
+                    "image_url": x.image_url,
+                    "image_date": x.image_date,
+                    "sample": x.sample
+                }
+                xtal_list.append(response)
+            res = {"xtal_list": xtal_list}
+            return res
+        except Exception:
+            logging.getLogger("MX3.HWR").exception("Could not get crystal List")
+            return {"xtal_list": xtal_list}
+
 
 def queue_mount_sample(view, data_model, centring_done_cb, async_result):
     from mxcube3.routes import signals
     from mxcube3 import mxcube
 
     HWR.beamline.sample_view.clear_all()
     logging.getLogger("user_level_log").info("Loading sample ...")
@@ -368,37 +397,30 @@
         "dewarLocation": loc[0],
         "sampleBarcode": data_model.code,
         "sampleId": data_model.lims_id,
         "sessionId": HWR.beamline.session.session_id,
         "startTime": time.strftime("%Y-%m-%d %H:%M:%S"),
     }
 
-    # This is a possible solution how to deal with two devices that
-    # can move sample on beam (sample changer, plate holder, in future
-    # also harvester)
-    # TODO make sample_Changer_one, sample_changer_two
-    if HWR.beamline.diffractometer.in_plate_mode():
-        sample_mount_device = HWR.beamline.plate_manipulator
-    else:
-        sample_mount_device = HWR.beamline.sample_changer
+    # devices that can move sample on beam
+    # (sample changer, plate holder)
+    # PlateManipulator is being consider as Sample changer
+    sample_mount_device = HWR.beamline.sample_changer
 
     if (
         sample_mount_device.get_loaded_sample()
         and sample_mount_device.get_loaded_sample().get_address() == data_model.loc_str
     ):
         return
 
     if hasattr(sample_mount_device, "__TYPE__"):
         if sample_mount_device.__TYPE__ in ["Marvin", "CATS"]:
             element = "%d:%02d" % loc
             sample = {"location": element, "sampleID": element}
             mxcube.sample_changer.mount_sample_clean_up(sample)
-        elif sample_mount_device.__TYPE__ == "PlateManipulator":
-            sample = {"location": data_model.loc_str, "sampleID": data_model.loc_str}
-            mxcube.sample_changer.mount_sample_clean_up(sample)
         else:
             sample = {"location": data_model.loc_str, "sampleID": data_model.loc_str}
 
             try:
                 res = mxcube.sample_changer.mount_sample_clean_up(sample)
             except RuntimeError:
                 res = False
```

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/sampleview.py` & `mxcubeweb-1.55.0/mxcube3/core/components/sampleview.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/user/database.py` & `mxcubeweb-1.55.0/mxcube3/core/components/user/database.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/user/usermanager.py` & `mxcubeweb-1.55.0/mxcube3/core/components/user/usermanager.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/components/workflow.py` & `mxcubeweb-1.55.0/mxcube3/core/components/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/models/adaptermodels.py` & `mxcubeweb-1.55.0/mxcube3/core/models/adaptermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/models/configmodels.py` & `mxcubeweb-1.55.0/mxcube3/core/models/configmodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/models/usermodels.py` & `mxcubeweb-1.55.0/mxcube3/core/models/usermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/util/adapterutils.py` & `mxcubeweb-1.55.0/mxcube3/core/util/adapterutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/util/convertutils.py` & `mxcubeweb-1.55.0/mxcube3/core/util/convertutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/util/fsutils.py` & `mxcubeweb-1.55.0/mxcube3/core/util/fsutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/core/util/networkutils.py` & `mxcubeweb-1.55.0/mxcube3/core/util/networkutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/logging_handler.py` & `mxcubeweb-1.55.0/mxcube3/logging_handler.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/beamline.py` & `mxcubeweb-1.55.0/mxcube3/routes/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/detector.py` & `mxcubeweb-1.55.0/mxcube3/routes/detector.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/diffractometer.py` & `mxcubeweb-1.55.0/mxcube3/routes/diffractometer.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/gphl_workflow.py` & `mxcubeweb-1.55.0/mxcube3/routes/gphl_workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/lims.py` & `mxcubeweb-1.55.0/mxcube3/routes/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/log.py` & `mxcubeweb-1.55.0/mxcube3/routes/log.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/login.py` & `mxcubeweb-1.55.0/mxcube3/routes/login.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/main.py` & `mxcubeweb-1.55.0/mxcube3/routes/main.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/mockups.py` & `mxcubeweb-1.55.0/mxcube3/routes/mockups.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/queue.py` & `mxcubeweb-1.55.0/mxcube3/routes/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/ra.py` & `mxcubeweb-1.55.0/mxcube3/routes/ra.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/samplecentring.py` & `mxcubeweb-1.55.0/mxcube3/routes/samplecentring.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/samplechanger.py` & `mxcubeweb-1.55.0/mxcube3/routes/samplechanger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 
     @bp.route("/samples_list", methods=["GET"])
     @server.restrict
     def get_sample_list():
         app.sample_changer.get_sample_list()
         return jsonify(app.lims.sample_list_get())
 
+    @bp.route("/sync_with_crims", methods=["GET"])
+    @server.require_control
+    @server.restrict
+    def sync_with_crims():
+        return app.sample_changer.sync_with_crims()
+
     @bp.route("/state", methods=["GET"])
     @server.restrict
     def get_sc_state():
         state = HWR.beamline.sample_changer.get_status().upper()
         return jsonify({"state": state})
 
     @bp.route("/loaded_sample", methods=["GET"])
```

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/signals.py` & `mxcubeweb-1.55.0/mxcube3/routes/signals.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/routes/workflow.py` & `mxcubeweb-1.55.0/mxcube3/routes/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/server.py` & `mxcubeweb-1.55.0/mxcube3/server.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/state_storage.py` & `mxcubeweb-1.55.0/mxcube3/state_storage.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/templates/characterisation-results.js` & `mxcubeweb-1.55.0/mxcube3/templates/characterisation-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/templates/data-collection-results.html` & `mxcubeweb-1.55.0/mxcube3/templates/data-collection-results.html`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/templates/precompiled.templates.min.js` & `mxcubeweb-1.55.0/mxcube3/templates/precompiled.templates.min.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/templates/workflow-results.js` & `mxcubeweb-1.55.0/mxcube3/templates/workflow-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/mxcube3/video/websocket-relay.js` & `mxcubeweb-1.55.0/mxcube3/video/websocket-relay.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.54.0/pyproject.toml` & `mxcubeweb-1.55.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcubeweb"
-version = "1.54.0"
+version = "1.55.0"
 license = "LGPL-3.0-or-later"
 description = "MXCuBE Web user interface"
 authors = ["The MXCuBE collaboration <mxcube@esrf.fr>"]
 maintainers = [
     "MXCuBE collaboration <mxcube@esrf.fr>",
 ]
 readme = "README.md"
```

### Comparing `mxcubeweb-1.54.0/PKG-INFO` & `mxcubeweb-1.55.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcubeweb
-Version: 1.54.0
+Version: 1.55.0
 Summary: MXCuBE Web user interface
 Home-page: http://github.com/mxcube/mxcubeweb
 License: LGPL-3.0-or-later
 Keywords: mxcube,mxcube3,mxcubeweb
 Author: The MXCuBE collaboration
 Author-email: mxcube@esrf.fr
 Maintainer: MXCuBE collaboration
```

