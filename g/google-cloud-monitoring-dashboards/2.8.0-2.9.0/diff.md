# Comparing `tmp/google-cloud-monitoring-dashboards-2.8.0.tar.gz` & `tmp/google-cloud-monitoring-dashboards-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-monitoring-dashboards-2.8.0.tar", last modified: Thu Oct 27 19:30:42 2022, max compression
+gzip compressed data, was "google-cloud-monitoring-dashboards-2.9.0.tar", last modified: Wed Dec 14 21:38:36 2022, max compression
```

## Comparing `google-cloud-monitoring-dashboards-2.8.0.tar` & `google-cloud-monitoring-dashboards-2.9.0.tar`

### file list

```diff
@@ -1,111 +1,114 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4949 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4055 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.900853 google-cloud-monitoring-dashboards-2.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.900853 google-cloud-monitoring-dashboards-2.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.904853 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/
--rw-rw-r--   0 root         (0)     1003     4140 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/__init__.py
--rw-rw-r--   0 root         (0)     1003       88 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.900853 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.908854 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/
--rw-rw-r--   0 root         (0)     1003    21274 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/common.proto
--rw-rw-r--   0 root         (0)     1003     2628 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/dashboard.proto
--rw-rw-r--   0 root         (0)     1003     6417 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/dashboards_service.proto
--rw-rw-r--   0 root         (0)     1003     1009 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/drilldowns.proto
--rw-rw-r--   0 root         (0)     1003     2834 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/layouts.proto
--rw-rw-r--   0 root         (0)     1003     6215 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/metrics.proto
--rw-rw-r--   0 root         (0)     1003     4429 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/scorecard.proto
--rw-rw-r--   0 root         (0)     1003      961 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/service.proto
--rw-rw-r--   0 root         (0)     1003     1402 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/text.proto
--rw-rw-r--   0 root         (0)     1003     1803 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/widget.proto
--rw-rw-r--   0 root         (0)     1003     5347 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/xychart.proto
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.908854 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/
--rw-rw-r--   0 root         (0)     1003     2869 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1812 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       88 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.908854 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.908854 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/
--rw-rw-r--   0 root         (0)     1003      781 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27079 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    36977 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/client.py
--rw-rw-r--   0 root         (0)     1003     6041 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.908854 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8268 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17749 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18114 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.912855 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/
--rw-rw-r--   0 root         (0)     1003     2327 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1186 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/alertchart.py
--rw-rw-r--   0 root         (0)     1003     1206 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/collapsible_group.py
--rw-rw-r--   0 root         (0)     1003    12296 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     4554 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboard.py
--rw-rw-r--   0 root         (0)     1003     2275 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboard_filter.py
--rw-rw-r--   0 root         (0)     1003     5202 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboards_service.py
--rw-rw-r--   0 root         (0)     1003      745 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/drilldowns.py
--rw-rw-r--   0 root         (0)     1003     6708 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/layouts.py
--rw-rw-r--   0 root         (0)     1003     1622 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/logs_panel.py
--rw-rw-r--   0 root         (0)     1003    11133 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/metrics.py
--rw-rw-r--   0 root         (0)     1003     6416 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/scorecard.py
--rw-rw-r--   0 root         (0)     1003      745 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     3426 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/table.py
--rw-rw-r--   0 root         (0)     1003     1168 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/table_display_options.py
--rw-rw-r--   0 root         (0)     1003     1404 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/text.py
--rw-rw-r--   0 root         (0)     1003     4799 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/widget.py
--rw-rw-r--   0 root         (0)     1003     6765 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/xychart.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.900853 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.912855 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard/
--rw-rw-r--   0 root         (0)     1003     3909 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard/__init__.py
--rw-rw-r--   0 root         (0)     1003       88 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.916856 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/
--rw-rw-r--   0 root         (0)     1003     2971 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003       88 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.916856 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/
--rw-rw-r--   0 root         (0)     1003      601 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.916856 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/
--rw-rw-r--   0 root         (0)     1003      783 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    15467 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    20561 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/client.py
--rw-rw-r--   0 root         (0)     1003     5843 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.916856 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/
--rw-rw-r--   0 root         (0)     1003     1224 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6391 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15219 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15270 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/
--rw-rw-r--   0 root         (0)     1003     1775 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11959 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     2862 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/dashboard.py
--rw-rw-r--   0 root         (0)     1003     4535 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/dashboards_service.py
--rw-rw-r--   0 root         (0)     1003      746 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/drilldowns.py
--rw-rw-r--   0 root         (0)     1003     4065 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/layouts.py
--rw-rw-r--   0 root         (0)     1003     8339 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/metrics.py
--rw-rw-r--   0 root         (0)     1003     5718 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/scorecard.py
--rw-rw-r--   0 root         (0)     1003      746 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003     1346 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/text.py
--rw-rw-r--   0 root         (0)     1003     2240 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/widget.py
--rw-rw-r--   0 root         (0)     1003     5669 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/xychart.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/
--rw-r--r--   0 root         (0)     1003     4949 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4698 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      232 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-27 19:30:42.000000 google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/scripts/
--rw-rw-r--   0 root         (0)     1003     6186 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/scripts/fixup_dashboard_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2605 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-27 19:30:42.920857 google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/dashboard_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/dashboard_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    88816 2022-10-27 19:26:56.000000 google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/dashboard_v1/test_dashboards_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.063870 google-cloud-monitoring-dashboards-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4962 2022-12-14 21:38:36.063870 google-cloud-monitoring-dashboards-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4055 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.043874 google-cloud-monitoring-dashboards-2.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.043874 google-cloud-monitoring-dashboards-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.047873 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/
+-rw-rw-r--   0 root         (0)     1003     4263 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.043874 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.047873 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/
+-rw-rw-r--   0 root         (0)     1003    21274 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/common.proto
+-rw-rw-r--   0 root         (0)     1003     2628 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/dashboard.proto
+-rw-rw-r--   0 root         (0)     1003     6417 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/dashboards_service.proto
+-rw-rw-r--   0 root         (0)     1003     1009 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/drilldowns.proto
+-rw-rw-r--   0 root         (0)     1003     2834 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/layouts.proto
+-rw-rw-r--   0 root         (0)     1003     6215 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/metrics.proto
+-rw-rw-r--   0 root         (0)     1003     4429 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/scorecard.proto
+-rw-rw-r--   0 root         (0)     1003      961 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/service.proto
+-rw-rw-r--   0 root         (0)     1003     1402 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/text.proto
+-rw-rw-r--   0 root         (0)     1003     1803 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/widget.proto
+-rw-rw-r--   0 root         (0)     1003     5347 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/xychart.proto
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.047873 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/
+-rw-rw-r--   0 root         (0)     1003     2992 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1818 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.047873 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.051872 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/
+-rw-rw-r--   0 root         (0)     1003      781 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27547 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37515 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6041 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.051872 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8154 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17849 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18201 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2327 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1243 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/alertchart.py
+-rw-rw-r--   0 root         (0)     1003     1264 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/collapsible_group.py
+-rw-rw-r--   0 root         (0)     1003    12455 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     4809 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboard.py
+-rw-rw-r--   0 root         (0)     1003     2354 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboard_filter.py
+-rw-rw-r--   0 root         (0)     1003     5400 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboards_service.py
+-rw-rw-r--   0 root         (0)     1003      745 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/drilldowns.py
+-rw-rw-r--   0 root         (0)     1003     7039 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/layouts.py
+-rw-rw-r--   0 root         (0)     1003     1708 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/logs_panel.py
+-rw-rw-r--   0 root         (0)     1003    11529 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/metrics.py
+-rw-rw-r--   0 root         (0)     1003     6678 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/scorecard.py
+-rw-rw-r--   0 root         (0)     1003      745 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     3656 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/table.py
+-rw-rw-r--   0 root         (0)     1003     1249 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/table_display_options.py
+-rw-rw-r--   0 root         (0)     1003     1469 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/text.py
+-rw-rw-r--   0 root         (0)     1003     5042 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/widget.py
+-rw-rw-r--   0 root         (0)     1003     7094 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/xychart.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.043874 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard/
+-rw-rw-r--   0 root         (0)     1003     3909 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard/__init__.py
+-rw-rw-r--   0 root         (0)     1003       88 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/
+-rw-rw-r--   0 root         (0)     1003     2971 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003       88 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/
+-rw-rw-r--   0 root         (0)     1003      601 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/
+-rw-rw-r--   0 root         (0)     1003      783 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    15467 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    20561 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5843 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.055871 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1224 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6391 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15219 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15270 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1775 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11959 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     2862 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/dashboard.py
+-rw-rw-r--   0 root         (0)     1003     4535 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/dashboards_service.py
+-rw-rw-r--   0 root         (0)     1003      746 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/drilldowns.py
+-rw-rw-r--   0 root         (0)     1003     4065 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/layouts.py
+-rw-rw-r--   0 root         (0)     1003     8339 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/metrics.py
+-rw-rw-r--   0 root         (0)     1003     5718 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/scorecard.py
+-rw-rw-r--   0 root         (0)     1003      746 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003     1346 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/text.py
+-rw-rw-r--   0 root         (0)     1003     2240 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/widget.py
+-rw-rw-r--   0 root         (0)     1003     5669 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/xychart.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/
+-rw-r--r--   0 root         (0)     1003     4962 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4885 2022-12-14 21:38:36.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      257 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-12-14 21:38:35.000000 google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-12-14 21:38:36.063870 google-cloud-monitoring-dashboards-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2922 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.059870 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/dashboard_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/dashboard_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    88870 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/dashboard_v1/test_dashboards_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-12-14 21:38:36.063870 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/monitoring_dashboard_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/monitoring_dashboard_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    88870 2022-12-14 21:35:23.000000 google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/monitoring_dashboard_v1/test_dashboards_service.py
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/LICENSE` & `google-cloud-monitoring-dashboards-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/MANIFEST.in` & `google-cloud-monitoring-dashboards-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/PKG-INFO` & `google-cloud-monitoring-dashboards-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring-dashboards
-Version: 2.8.0
-Summary: Monitoring Dashboards API client library
+Version: 2.9.0
+Summary: Google Cloud Monitoring Dashboards API client library
 Home-page: https://github.com/googleapis/python-monitoring-dashboards
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/README.rst` & `google-cloud-monitoring-dashboards-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.monitoring_dashboard import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from google.cloud.monitoring_dashboard_v1.services.dashboards_service.client import (
     DashboardsServiceClient,
 )
 from google.cloud.monitoring_dashboard_v1.services.dashboards_service.async_client import (
     DashboardsServiceAsyncClient,
 )
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/common.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/common.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/dashboard.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/dashboard.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/dashboards_service.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/dashboards_service.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/drilldowns.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/drilldowns.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/layouts.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/layouts.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/metrics.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/metrics.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/scorecard.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/scorecard.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/service.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/service.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/text.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/text.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/widget.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/widget.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard/v1/proto/xychart.proto` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard/v1/proto/xychart.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from google.cloud.monitoring_dashboard import gapic_version as package_version
+
+__version__ = package_version.__version__
+
 
 from .services.dashboards_service import DashboardsServiceClient
 from .services.dashboards_service import DashboardsServiceAsyncClient
 
 from .types.alertchart import AlertChart
 from .types.collapsible_group import CollapsibleGroup
 from .types.common import Aggregation
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/gapic_metadata.json` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/gapic_metadata.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'libraryPackage'": "'google.cloud.monitoring_dashboard_v1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.monitoring.dashboard_v1",
+    "libraryPackage": "google.cloud.monitoring_dashboard_v1",
     "protoPackage": "google.monitoring.dashboard.v1",
     "schema": "1.0",
     "services": {
         "DashboardsService": {
             "clients": {
                 "grpc": {
                     "libraryClient": "DashboardsServiceClient",
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/async_client.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
+
+from google.cloud.monitoring_dashboard_v1 import gapic_version as package_version
 
 from google.api_core.client_options import ClientOptions
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
@@ -163,17 +174,17 @@
     get_transport_class = functools.partial(
         type(DashboardsServiceClient).get_transport_class, type(DashboardsServiceClient)
     )
 
     def __init__(
         self,
         *,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         transport: Union[str, DashboardsServiceTransport] = "grpc_asyncio",
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the dashboards service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
@@ -209,18 +220,20 @@
             transport=transport,
             client_options=client_options,
             client_info=client_info,
         )
 
     async def create_dashboard(
         self,
-        request: Union[dashboards_service.CreateDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.CreateDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Creates a new custom dashboard. For examples on how you can use
         this API to create dashboards, see `Managing dashboards by
         API <https://cloud.google.com/monitoring/dashboards/api-dashboard>`__.
         This method requires the ``monitoring.dashboards.create``
         permission on the specified project. For more information about
@@ -232,37 +245,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             async def sample_create_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceAsyncClient()
+                client = monitoring_dashboard_v1.DashboardsServiceAsyncClient()
 
                 # Initialize request argument(s)
-                dashboard = dashboard_v1.Dashboard()
+                dashboard = monitoring_dashboard_v1.Dashboard()
                 dashboard.display_name = "display_name_value"
 
-                request = dashboard_v1.CreateDashboardRequest(
+                request = monitoring_dashboard_v1.CreateDashboardRequest(
                     parent="parent_value",
                     dashboard=dashboard,
                 )
 
                 # Make the request
                 response = await client.create_dashboard(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.monitoring_dashboard_v1.types.CreateDashboardRequest, dict]):
+            request (Optional[Union[google.cloud.monitoring_dashboard_v1.types.CreateDashboardRequest, dict]]):
                 The request object. The `CreateDashboard` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -300,18 +313,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def list_dashboards(
         self,
-        request: Union[dashboards_service.ListDashboardsRequest, dict] = None,
+        request: Optional[Union[dashboards_service.ListDashboardsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDashboardsAsyncPager:
         r"""Lists the existing dashboards.
 
         This method requires the ``monitoring.dashboards.list``
         permission on the specified project. For more information, see
         `Cloud Identity and Access
@@ -322,34 +335,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             async def sample_list_dashboards():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceAsyncClient()
+                client = monitoring_dashboard_v1.DashboardsServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.ListDashboardsRequest(
+                request = monitoring_dashboard_v1.ListDashboardsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_dashboards(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.monitoring_dashboard_v1.types.ListDashboardsRequest, dict]):
+            request (Optional[Union[google.cloud.monitoring_dashboard_v1.types.ListDashboardsRequest, dict]]):
                 The request object. The `ListDashboards` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -396,18 +409,18 @@
         )
 
         # Done; return the response.
         return response
 
     async def get_dashboard(
         self,
-        request: Union[dashboards_service.GetDashboardRequest, dict] = None,
+        request: Optional[Union[dashboards_service.GetDashboardRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Fetches a specific dashboard.
 
         This method requires the ``monitoring.dashboards.get``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -418,33 +431,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             async def sample_get_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceAsyncClient()
+                client = monitoring_dashboard_v1.DashboardsServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.GetDashboardRequest(
+                request = monitoring_dashboard_v1.GetDashboardRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_dashboard(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.monitoring_dashboard_v1.types.GetDashboardRequest, dict]):
+            request (Optional[Union[google.cloud.monitoring_dashboard_v1.types.GetDashboardRequest, dict]]):
                 The request object. The `GetDashboard` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -482,18 +495,20 @@
         )
 
         # Done; return the response.
         return response
 
     async def delete_dashboard(
         self,
-        request: Union[dashboards_service.DeleteDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.DeleteDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes an existing custom dashboard.
 
         This method requires the ``monitoring.dashboards.delete``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -504,30 +519,30 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             async def sample_delete_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceAsyncClient()
+                client = monitoring_dashboard_v1.DashboardsServiceAsyncClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.DeleteDashboardRequest(
+                request = monitoring_dashboard_v1.DeleteDashboardRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 await client.delete_dashboard(request=request)
 
         Args:
-            request (Union[google.cloud.monitoring_dashboard_v1.types.DeleteDashboardRequest, dict]):
+            request (Optional[Union[google.cloud.monitoring_dashboard_v1.types.DeleteDashboardRequest, dict]]):
                 The request object. The `DeleteDashboard` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
@@ -554,18 +569,20 @@
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
     async def update_dashboard(
         self,
-        request: Union[dashboards_service.UpdateDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.UpdateDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Replaces an existing custom dashboard with a new definition.
 
         This method requires the ``monitoring.dashboards.update``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -576,36 +593,36 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             async def sample_update_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceAsyncClient()
+                client = monitoring_dashboard_v1.DashboardsServiceAsyncClient()
 
                 # Initialize request argument(s)
-                dashboard = dashboard_v1.Dashboard()
+                dashboard = monitoring_dashboard_v1.Dashboard()
                 dashboard.display_name = "display_name_value"
 
-                request = dashboard_v1.UpdateDashboardRequest(
+                request = monitoring_dashboard_v1.UpdateDashboardRequest(
                     dashboard=dashboard,
                 )
 
                 # Make the request
                 response = await client.update_dashboard(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.monitoring_dashboard_v1.types.UpdateDashboardRequest, dict]):
+            request (Optional[Union[google.cloud.monitoring_dashboard_v1.types.UpdateDashboardRequest, dict]]):
                 The request object. The `UpdateDashboard` request.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
@@ -650,18 +667,13 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-monitoring-dashboard",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("DashboardsServiceAsyncClient",)
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/client.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
-from typing import Dict, Mapping, Optional, Sequence, Tuple, Type, Union
-import pkg_resources
+from typing import (
+    Dict,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+from google.cloud.monitoring_dashboard_v1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -56,15 +68,15 @@
         OrderedDict()
     )  # type: Dict[str, Type[DashboardsServiceTransport]]
     _transport_registry["grpc"] = DashboardsServiceGrpcTransport
     _transport_registry["grpc_asyncio"] = DashboardsServiceGrpcAsyncIOTransport
 
     def get_transport_class(
         cls,
-        label: str = None,
+        label: Optional[str] = None,
     ) -> Type[DashboardsServiceTransport]:
         """Returns an appropriate transport class.
 
         Args:
             label: The name of the desired transport. If none is
                 provided, then the first transport in the registry is used.
 
@@ -347,30 +359,30 @@
 
         return api_endpoint, client_cert_source
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, DashboardsServiceTransport, None] = None,
-        client_options: Optional[client_options_lib.ClientOptions] = None,
+        transport: Optional[Union[str, DashboardsServiceTransport]] = None,
+        client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the dashboards service client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
             transport (Union[str, DashboardsServiceTransport]): The
                 transport to use. If set to None, a transport is chosen
                 automatically.
-            client_options (google.api_core.client_options.ClientOptions): Custom options for the
+            client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]): Custom options for the
                 client. It won't take effect if a ``transport`` instance is provided.
                 (1) The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client. GOOGLE_API_USE_MTLS_ENDPOINT
                 environment variable can also be used to override the endpoint:
                 "always" (always use the default mTLS endpoint), "never" (always
                 use the default regular endpoint) and "auto" (auto switch to the
                 default mTLS endpoint if client certificate is present, this is
@@ -392,14 +404,15 @@
             google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
                 creation failed for any reason.
         """
         if isinstance(client_options, dict):
             client_options = client_options_lib.from_dict(client_options)
         if client_options is None:
             client_options = client_options_lib.ClientOptions()
+        client_options = cast(client_options_lib.ClientOptions, client_options)
 
         api_endpoint, client_cert_source_func = self.get_mtls_endpoint_and_cert_source(
             client_options
         )
 
         api_key_value = getattr(client_options, "api_key", None)
         if api_key_value and credentials:
@@ -444,18 +457,20 @@
                 client_info=client_info,
                 always_use_jwt_access=True,
                 api_audience=client_options.api_audience,
             )
 
     def create_dashboard(
         self,
-        request: Union[dashboards_service.CreateDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.CreateDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Creates a new custom dashboard. For examples on how you can use
         this API to create dashboards, see `Managing dashboards by
         API <https://cloud.google.com/monitoring/dashboards/api-dashboard>`__.
         This method requires the ``monitoring.dashboards.create``
         permission on the specified project. For more information about
@@ -467,25 +482,25 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             def sample_create_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceClient()
+                client = monitoring_dashboard_v1.DashboardsServiceClient()
 
                 # Initialize request argument(s)
-                dashboard = dashboard_v1.Dashboard()
+                dashboard = monitoring_dashboard_v1.Dashboard()
                 dashboard.display_name = "display_name_value"
 
-                request = dashboard_v1.CreateDashboardRequest(
+                request = monitoring_dashboard_v1.CreateDashboardRequest(
                     parent="parent_value",
                     dashboard=dashboard,
                 )
 
                 # Make the request
                 response = client.create_dashboard(request=request)
 
@@ -536,18 +551,18 @@
         )
 
         # Done; return the response.
         return response
 
     def list_dashboards(
         self,
-        request: Union[dashboards_service.ListDashboardsRequest, dict] = None,
+        request: Optional[Union[dashboards_service.ListDashboardsRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDashboardsPager:
         r"""Lists the existing dashboards.
 
         This method requires the ``monitoring.dashboards.list``
         permission on the specified project. For more information, see
         `Cloud Identity and Access
@@ -558,22 +573,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             def sample_list_dashboards():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceClient()
+                client = monitoring_dashboard_v1.DashboardsServiceClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.ListDashboardsRequest(
+                request = monitoring_dashboard_v1.ListDashboardsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_dashboards(request=request)
 
                 # Handle the response
@@ -633,18 +648,18 @@
         )
 
         # Done; return the response.
         return response
 
     def get_dashboard(
         self,
-        request: Union[dashboards_service.GetDashboardRequest, dict] = None,
+        request: Optional[Union[dashboards_service.GetDashboardRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Fetches a specific dashboard.
 
         This method requires the ``monitoring.dashboards.get``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -655,22 +670,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             def sample_get_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceClient()
+                client = monitoring_dashboard_v1.DashboardsServiceClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.GetDashboardRequest(
+                request = monitoring_dashboard_v1.GetDashboardRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_dashboard(request=request)
 
                 # Handle the response
@@ -720,18 +735,20 @@
         )
 
         # Done; return the response.
         return response
 
     def delete_dashboard(
         self,
-        request: Union[dashboards_service.DeleteDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.DeleteDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
         r"""Deletes an existing custom dashboard.
 
         This method requires the ``monitoring.dashboards.delete``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -742,22 +759,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             def sample_delete_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceClient()
+                client = monitoring_dashboard_v1.DashboardsServiceClient()
 
                 # Initialize request argument(s)
-                request = dashboard_v1.DeleteDashboardRequest(
+                request = monitoring_dashboard_v1.DeleteDashboardRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 client.delete_dashboard(request=request)
 
         Args:
@@ -793,18 +810,20 @@
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
     def update_dashboard(
         self,
-        request: Union[dashboards_service.UpdateDashboardRequest, dict] = None,
+        request: Optional[
+            Union[dashboards_service.UpdateDashboardRequest, dict]
+        ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: float = None,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dashboard.Dashboard:
         r"""Replaces an existing custom dashboard with a new definition.
 
         This method requires the ``monitoring.dashboards.update``
         permission on the specified dashboard. For more information, see
         `Cloud Identity and Access
@@ -815,25 +834,25 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.monitoring import dashboard_v1
+            from google.cloud import monitoring_dashboard_v1
 
             def sample_update_dashboard():
                 # Create a client
-                client = dashboard_v1.DashboardsServiceClient()
+                client = monitoring_dashboard_v1.DashboardsServiceClient()
 
                 # Initialize request argument(s)
-                dashboard = dashboard_v1.Dashboard()
+                dashboard = monitoring_dashboard_v1.Dashboard()
                 dashboard.display_name = "display_name_value"
 
-                request = dashboard_v1.UpdateDashboardRequest(
+                request = monitoring_dashboard_v1.UpdateDashboardRequest(
                     dashboard=dashboard,
                 )
 
                 # Make the request
                 response = client.update_dashboard(request=request)
 
                 # Handle the response
@@ -897,18 +916,13 @@
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-monitoring-dashboard",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 __all__ = ("DashboardsServiceClient",)
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/pagers.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/base.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,36 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import abc
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Union
-import pkg_resources
+
+from google.cloud.monitoring_dashboard_v1 import gapic_version as package_version
 
 import google.auth  # type: ignore
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import dashboard
 from google.cloud.monitoring_dashboard_v1.types import dashboards_service
 from google.protobuf import empty_pb2  # type: ignore
 
-try:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
-        gapic_version=pkg_resources.get_distribution(
-            "google-monitoring-dashboard",
-        ).version,
-    )
-except pkg_resources.DistributionNotFound:
-    DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
+DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
+    gapic_version=package_version.__version__
+)
 
 
 class DashboardsServiceTransport(abc.ABC):
     """Abstract transport class for DashboardsService."""
 
     AUTH_SCOPES = (
         "https://www.googleapis.com/auth/cloud-platform",
@@ -51,15 +47,15 @@
 
     DEFAULT_HOST: str = "monitoring.googleapis.com"
 
     def __init__(
         self,
         *,
         host: str = DEFAULT_HOST,
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
         **kwargs,
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
     _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "monitoring.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
-        scopes: Sequence[str] = None,
-        channel: grpc.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        channel: Optional[grpc.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
@@ -180,16 +180,16 @@
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
     @classmethod
     def create_channel(
         cls,
         host: str = "monitoring.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
-        credentials_file: str = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> grpc.Channel:
         """Create and return a gRPC channel object.
         Args:
             host (Optional[str]): The host for the channel to use.
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     _grpc_channel: aio.Channel
     _stubs: Dict[str, Callable] = {}
 
     @classmethod
     def create_channel(
         cls,
         host: str = "monitoring.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         **kwargs,
     ) -> aio.Channel:
         """Create and return a gRPC AsyncIO channel object.
         Args:
@@ -91,23 +91,23 @@
             **kwargs,
         )
 
     def __init__(
         self,
         *,
         host: str = "monitoring.googleapis.com",
-        credentials: ga_credentials.Credentials = None,
+        credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: aio.Channel = None,
-        api_mtls_endpoint: str = None,
-        client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
-        ssl_channel_credentials: grpc.ChannelCredentials = None,
-        client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
-        quota_project_id=None,
+        channel: Optional[aio.Channel] = None,
+        api_mtls_endpoint: Optional[str] = None,
+        client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
+        client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
+        quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
         api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/alertchart.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/alertchart.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
         "AlertChart",
@@ -33,14 +35,14 @@
             is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/alertPolicies/[ALERT_POLICY_ID]
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/collapsible_group.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/collapsible_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
         "CollapsibleGroup",
@@ -31,14 +33,14 @@
 
     Attributes:
         collapsed (bool):
             The collapsed state of the widget on first
             page load.
     """
 
-    collapsed = proto.Field(
+    collapsed: bool = proto.Field(
         proto.BOOL,
         number=1,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/common.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.protobuf import duration_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
@@ -108,15 +110,15 @@
 
             Time series data must first be aligned (see
             ``per_series_aligner``) in order to perform cross-time
             series reduction. If ``cross_series_reducer`` is specified,
             then ``per_series_aligner`` must be specified, and must not
             be ``ALIGN_NONE``. An ``alignment_period`` must also be
             specified; otherwise, an error is returned.
-        group_by_fields (Sequence[str]):
+        group_by_fields (MutableSequence[str]):
             The set of fields to preserve when ``cross_series_reducer``
             is specified. The ``group_by_fields`` determine how the time
             series are partitioned into subsets prior to applying the
             aggregation operation. Each subset contains time series that
             have the same value for each of the grouping fields. Each
             individual time series is a member of exactly one subset.
             The ``cross_series_reducer`` is applied to each subset of
@@ -182,30 +184,30 @@
         REDUCE_COUNT_FALSE = 15
         REDUCE_FRACTION_TRUE = 8
         REDUCE_PERCENTILE_99 = 9
         REDUCE_PERCENTILE_95 = 10
         REDUCE_PERCENTILE_50 = 11
         REDUCE_PERCENTILE_05 = 12
 
-    alignment_period = proto.Field(
+    alignment_period: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=1,
         message=duration_pb2.Duration,
     )
-    per_series_aligner = proto.Field(
+    per_series_aligner: Aligner = proto.Field(
         proto.ENUM,
         number=2,
         enum=Aligner,
     )
-    cross_series_reducer = proto.Field(
+    cross_series_reducer: Reducer = proto.Field(
         proto.ENUM,
         number=4,
         enum=Reducer,
     )
-    group_by_fields = proto.RepeatedField(
+    group_by_fields: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=5,
     )
 
 
 class PickTimeSeriesFilter(proto.Message):
     r"""Describes a ranking-based time series filter. Each input time series
@@ -244,24 +246,24 @@
 
     class Direction(proto.Enum):
         r"""Describes the ranking directions."""
         DIRECTION_UNSPECIFIED = 0
         TOP = 1
         BOTTOM = 2
 
-    ranking_method = proto.Field(
+    ranking_method: Method = proto.Field(
         proto.ENUM,
         number=1,
         enum=Method,
     )
-    num_time_series = proto.Field(
+    num_time_series: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    direction = proto.Field(
+    direction: Direction = proto.Field(
         proto.ENUM,
         number=3,
         enum=Direction,
     )
 
 
 class StatisticalTimeSeriesFilter(proto.Message):
@@ -283,19 +285,19 @@
     """
 
     class Method(proto.Enum):
         r"""The filter methods that can be applied to a stream."""
         METHOD_UNSPECIFIED = 0
         METHOD_CLUSTER_OUTLIER = 1
 
-    ranking_method = proto.Field(
+    ranking_method: Method = proto.Field(
         proto.ENUM,
         number=1,
         enum=Method,
     )
-    num_time_series = proto.Field(
+    num_time_series: int = proto.Field(
         proto.INT32,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboard.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import dashboard_filter
 from google.cloud.monitoring_dashboard_v1.types import layouts
 
 
 __protobuf__ = proto.module(
@@ -71,63 +73,65 @@
 
             This field is a member of `oneof`_ ``layout``.
         column_layout (google.cloud.monitoring_dashboard_v1.types.ColumnLayout):
             The content is divided into equally spaced
             columns and the widgets are arranged vertically.
 
             This field is a member of `oneof`_ ``layout``.
-        dashboard_filters (Sequence[google.cloud.monitoring_dashboard_v1.types.DashboardFilter]):
+        dashboard_filters (MutableSequence[google.cloud.monitoring_dashboard_v1.types.DashboardFilter]):
             Filters to reduce the amount of data charted
             based on the filter criteria.
-        labels (Mapping[str, str]):
+        labels (MutableMapping[str, str]):
             Labels applied to the dashboard
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    display_name = proto.Field(
+    display_name: str = proto.Field(
         proto.STRING,
         number=2,
     )
-    etag = proto.Field(
+    etag: str = proto.Field(
         proto.STRING,
         number=4,
     )
-    grid_layout = proto.Field(
+    grid_layout: layouts.GridLayout = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="layout",
         message=layouts.GridLayout,
     )
-    mosaic_layout = proto.Field(
+    mosaic_layout: layouts.MosaicLayout = proto.Field(
         proto.MESSAGE,
         number=6,
         oneof="layout",
         message=layouts.MosaicLayout,
     )
-    row_layout = proto.Field(
+    row_layout: layouts.RowLayout = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="layout",
         message=layouts.RowLayout,
     )
-    column_layout = proto.Field(
+    column_layout: layouts.ColumnLayout = proto.Field(
         proto.MESSAGE,
         number=9,
         oneof="layout",
         message=layouts.ColumnLayout,
     )
-    dashboard_filters = proto.RepeatedField(
+    dashboard_filters: MutableSequence[
+        dashboard_filter.DashboardFilter
+    ] = proto.RepeatedField(
         proto.MESSAGE,
         number=11,
         message=dashboard_filter.DashboardFilter,
     )
-    labels = proto.MapField(
+    labels: MutableMapping[str, str] = proto.MapField(
         proto.STRING,
         proto.STRING,
         number=12,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboard_filter.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboard_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
         "DashboardFilter",
@@ -52,28 +54,28 @@
         FILTER_TYPE_UNSPECIFIED = 0
         RESOURCE_LABEL = 1
         METRIC_LABEL = 2
         USER_METADATA_LABEL = 3
         SYSTEM_METADATA_LABEL = 4
         GROUP = 5
 
-    label_key = proto.Field(
+    label_key: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    template_variable = proto.Field(
+    template_variable: str = proto.Field(
         proto.STRING,
         number=3,
     )
-    string_value = proto.Field(
+    string_value: str = proto.Field(
         proto.STRING,
         number=4,
         oneof="default_value",
     )
-    filter_type = proto.Field(
+    filter_type: FilterType = proto.Field(
         proto.ENUM,
         number=5,
         enum=FilterType,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/dashboards_service.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/dashboards_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import dashboard as gmd_dashboard
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
@@ -49,24 +51,24 @@
             Required. The initial dashboard
             specification.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually save it.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    dashboard = proto.Field(
+    dashboard: gmd_dashboard.Dashboard = proto.Field(
         proto.MESSAGE,
         number=2,
         message=gmd_dashboard.Dashboard,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 class ListDashboardsRequest(proto.Message):
     r"""The ``ListDashboards`` request.
@@ -86,51 +88,51 @@
         page_token (str):
             If this field is not empty then it must contain the
             ``nextPageToken`` value returned by a previous call to this
             method. Using this field causes the method to return
             additional results from the previous method call.
     """
 
-    parent = proto.Field(
+    parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    page_size = proto.Field(
+    page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
-    page_token = proto.Field(
+    page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
 class ListDashboardsResponse(proto.Message):
     r"""The ``ListDashboards`` request.
 
     Attributes:
-        dashboards (Sequence[google.cloud.monitoring_dashboard_v1.types.Dashboard]):
+        dashboards (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Dashboard]):
             The list of requested dashboards.
         next_page_token (str):
             If there are more results than have been returned, then this
             field is set to a non-empty value. To see the additional
             results, use that value as ``page_token`` in the next call
             to this method.
     """
 
     @property
     def raw_page(self):
         return self
 
-    dashboards = proto.RepeatedField(
+    dashboards: MutableSequence[gmd_dashboard.Dashboard] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=gmd_dashboard.Dashboard,
     )
-    next_page_token = proto.Field(
+    next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class GetDashboardRequest(proto.Message):
     r"""The ``GetDashboard`` request.
@@ -141,15 +143,15 @@
             one of:
 
             -  ``dashboards/[DASHBOARD_ID]`` (for system dashboards)
             -  ``projects/[PROJECT_ID_OR_NUMBER]/dashboards/[DASHBOARD_ID]``
                (for custom dashboards).
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class DeleteDashboardRequest(proto.Message):
     r"""The ``DeleteDashboard`` request.
@@ -159,15 +161,15 @@
             Required. The resource name of the Dashboard. The format is:
 
             ::
 
                 projects/[PROJECT_ID_OR_NUMBER]/dashboards/[DASHBOARD_ID]
     """
 
-    name = proto.Field(
+    name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class UpdateDashboardRequest(proto.Message):
     r"""The ``UpdateDashboard`` request.
@@ -177,19 +179,19 @@
             Required. The dashboard that will replace the
             existing dashboard.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually save it.
     """
 
-    dashboard = proto.Field(
+    dashboard: gmd_dashboard.Dashboard = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gmd_dashboard.Dashboard,
     )
-    validate_only = proto.Field(
+    validate_only: bool = proto.Field(
         proto.BOOL,
         number=3,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/drilldowns.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/drilldowns.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/layouts.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/layouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import widget as gmd_widget
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
@@ -35,24 +37,24 @@
     row-first strategy.
 
     Attributes:
         columns (int):
             The number of columns into which the view's
             width is divided. If omitted or set to zero, a
             system default will be used while rendering.
-        widgets (Sequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
+        widgets (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
             The informational elements that are arranged
             into the columns row-first.
     """
 
-    columns = proto.Field(
+    columns: int = proto.Field(
         proto.INT64,
         number=1,
     )
-    widgets = proto.RepeatedField(
+    widgets: MutableSequence[gmd_widget.Widget] = proto.RepeatedField(
         proto.MESSAGE,
         number=2,
         message=gmd_widget.Widget,
     )
 
 
 class MosaicLayout(proto.Message):
@@ -62,15 +64,15 @@
     in the grid.
 
     Attributes:
         columns (int):
             The number of columns in the mosaic grid. The
             number of columns must be between 1 and 12,
             inclusive.
-        tiles (Sequence[google.cloud.monitoring_dashboard_v1.types.MosaicLayout.Tile]):
+        tiles (MutableSequence[google.cloud.monitoring_dashboard_v1.types.MosaicLayout.Tile]):
             The tiles to display.
     """
 
     class Tile(proto.Message):
         r"""A single tile in the mosaic. The placement and size of the
         tile are configurable.
 
@@ -91,126 +93,126 @@
                 The height of the tile, measured in grid
                 blocks. Tiles must have a minimum height of 1.
             widget (google.cloud.monitoring_dashboard_v1.types.Widget):
                 The informational widget contained in the tile. For example
                 an ``XyChart``.
         """
 
-        x_pos = proto.Field(
+        x_pos: int = proto.Field(
             proto.INT32,
             number=1,
         )
-        y_pos = proto.Field(
+        y_pos: int = proto.Field(
             proto.INT32,
             number=2,
         )
-        width = proto.Field(
+        width: int = proto.Field(
             proto.INT32,
             number=3,
         )
-        height = proto.Field(
+        height: int = proto.Field(
             proto.INT32,
             number=4,
         )
-        widget = proto.Field(
+        widget: gmd_widget.Widget = proto.Field(
             proto.MESSAGE,
             number=5,
             message=gmd_widget.Widget,
         )
 
-    columns = proto.Field(
+    columns: int = proto.Field(
         proto.INT32,
         number=1,
     )
-    tiles = proto.RepeatedField(
+    tiles: MutableSequence[Tile] = proto.RepeatedField(
         proto.MESSAGE,
         number=3,
         message=Tile,
     )
 
 
 class RowLayout(proto.Message):
     r"""A simplified layout that divides the available space into
     rows and arranges a set of widgets horizontally in each row.
 
     Attributes:
-        rows (Sequence[google.cloud.monitoring_dashboard_v1.types.RowLayout.Row]):
+        rows (MutableSequence[google.cloud.monitoring_dashboard_v1.types.RowLayout.Row]):
             The rows of content to display.
     """
 
     class Row(proto.Message):
         r"""Defines the layout properties and content for a row.
 
         Attributes:
             weight (int):
                 The relative weight of this row. The row
                 weight is used to adjust the height of rows on
                 the screen (relative to peers). Greater the
                 weight, greater the height of the row on the
                 screen. If omitted, a value of 1 is used while
                 rendering.
-            widgets (Sequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
+            widgets (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
                 The display widgets arranged horizontally in
                 this row.
         """
 
-        weight = proto.Field(
+        weight: int = proto.Field(
             proto.INT64,
             number=1,
         )
-        widgets = proto.RepeatedField(
+        widgets: MutableSequence[gmd_widget.Widget] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message=gmd_widget.Widget,
         )
 
-    rows = proto.RepeatedField(
+    rows: MutableSequence[Row] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=Row,
     )
 
 
 class ColumnLayout(proto.Message):
     r"""A simplified layout that divides the available space into
     vertical columns and arranges a set of widgets vertically in
     each column.
 
     Attributes:
-        columns (Sequence[google.cloud.monitoring_dashboard_v1.types.ColumnLayout.Column]):
+        columns (MutableSequence[google.cloud.monitoring_dashboard_v1.types.ColumnLayout.Column]):
             The columns of content to display.
     """
 
     class Column(proto.Message):
         r"""Defines the layout properties and content for a column.
 
         Attributes:
             weight (int):
                 The relative weight of this column. The
                 column weight is used to adjust the width of
                 columns on the screen (relative to peers).
                 Greater the weight, greater the width of the
                 column on the screen. If omitted, a value of 1
                 is used while rendering.
-            widgets (Sequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
+            widgets (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Widget]):
                 The display widgets arranged vertically in
                 this column.
         """
 
-        weight = proto.Field(
+        weight: int = proto.Field(
             proto.INT64,
             number=1,
         )
-        widgets = proto.RepeatedField(
+        widgets: MutableSequence[gmd_widget.Widget] = proto.RepeatedField(
             proto.MESSAGE,
             number=2,
             message=gmd_widget.Widget,
         )
 
-    columns = proto.RepeatedField(
+    columns: MutableSequence[Column] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=Column,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/logs_panel.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/logs_panel.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
         "LogsPanel",
@@ -30,25 +32,25 @@
     Attributes:
         filter (str):
             A filter that chooses which log entries to return. See
             `Advanced Logs
             Queries <https://cloud.google.com/logging/docs/view/advanced-queries>`__.
             Only log entries that match the filter are returned. An
             empty filter matches all log entries.
-        resource_names (Sequence[str]):
+        resource_names (MutableSequence[str]):
             The names of logging resources to collect
             logs for. Currently only projects are supported.
             If empty, the widget will default to the host
             project.
     """
 
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    resource_names = proto.RepeatedField(
+    resource_names: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=2,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/metrics.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import common
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
@@ -73,37 +75,37 @@
             The unit of data contained in fetched time series. If
             non-empty, this unit will override any unit that accompanies
             fetched data. The format is the same as the
             ```unit`` <https://cloud.google.com/monitoring/api/ref_v3/rest/v3/projects.metricDescriptors>`__
             field in ``MetricDescriptor``.
     """
 
-    time_series_filter = proto.Field(
+    time_series_filter: "TimeSeriesFilter" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="source",
         message="TimeSeriesFilter",
     )
-    time_series_filter_ratio = proto.Field(
+    time_series_filter_ratio: "TimeSeriesFilterRatio" = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="source",
         message="TimeSeriesFilterRatio",
     )
-    time_series_query_language = proto.Field(
+    time_series_query_language: str = proto.Field(
         proto.STRING,
         number=3,
         oneof="source",
     )
-    prometheus_query = proto.Field(
+    prometheus_query: str = proto.Field(
         proto.STRING,
         number=6,
         oneof="source",
     )
-    unit_override = proto.Field(
+    unit_override: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class TimeSeriesFilter(proto.Message):
     r"""A filter that defines a subset of time series data that is displayed
@@ -138,35 +140,35 @@
             Statistics based time series filter.
             Note: This field is deprecated and completely
             ignored by the API.
 
             This field is a member of `oneof`_ ``output_filter``.
     """
 
-    filter = proto.Field(
+    filter: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    aggregation = proto.Field(
+    aggregation: common.Aggregation = proto.Field(
         proto.MESSAGE,
         number=2,
         message=common.Aggregation,
     )
-    secondary_aggregation = proto.Field(
+    secondary_aggregation: common.Aggregation = proto.Field(
         proto.MESSAGE,
         number=3,
         message=common.Aggregation,
     )
-    pick_time_series_filter = proto.Field(
+    pick_time_series_filter: common.PickTimeSeriesFilter = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="output_filter",
         message=common.PickTimeSeriesFilter,
     )
-    statistical_time_series_filter = proto.Field(
+    statistical_time_series_filter: common.StatisticalTimeSeriesFilter = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="output_filter",
         message=common.StatisticalTimeSeriesFilter,
     )
 
 
@@ -215,46 +217,46 @@
                 query.
             aggregation (google.cloud.monitoring_dashboard_v1.types.Aggregation):
                 By default, the raw time series data is
                 returned. Use this field to combine multiple
                 time series for different views of the data.
         """
 
-        filter = proto.Field(
+        filter: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        aggregation = proto.Field(
+        aggregation: common.Aggregation = proto.Field(
             proto.MESSAGE,
             number=2,
             message=common.Aggregation,
         )
 
-    numerator = proto.Field(
+    numerator: RatioPart = proto.Field(
         proto.MESSAGE,
         number=1,
         message=RatioPart,
     )
-    denominator = proto.Field(
+    denominator: RatioPart = proto.Field(
         proto.MESSAGE,
         number=2,
         message=RatioPart,
     )
-    secondary_aggregation = proto.Field(
+    secondary_aggregation: common.Aggregation = proto.Field(
         proto.MESSAGE,
         number=3,
         message=common.Aggregation,
     )
-    pick_time_series_filter = proto.Field(
+    pick_time_series_filter: common.PickTimeSeriesFilter = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="output_filter",
         message=common.PickTimeSeriesFilter,
     )
-    statistical_time_series_filter = proto.Field(
+    statistical_time_series_filter: common.StatisticalTimeSeriesFilter = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="output_filter",
         message=common.StatisticalTimeSeriesFilter,
     )
 
 
@@ -299,33 +301,33 @@
 
     class TargetAxis(proto.Enum):
         r"""An axis identifier."""
         TARGET_AXIS_UNSPECIFIED = 0
         Y1 = 1
         Y2 = 2
 
-    label = proto.Field(
+    label: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    value = proto.Field(
+    value: float = proto.Field(
         proto.DOUBLE,
         number=2,
     )
-    color = proto.Field(
+    color: Color = proto.Field(
         proto.ENUM,
         number=3,
         enum=Color,
     )
-    direction = proto.Field(
+    direction: Direction = proto.Field(
         proto.ENUM,
         number=4,
         enum=Direction,
     )
-    target_axis = proto.Field(
+    target_axis: TargetAxis = proto.Field(
         proto.ENUM,
         number=5,
         enum=TargetAxis,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/scorecard.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/scorecard.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import metrics
 from google.protobuf import duration_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -48,55 +50,57 @@
 
             This field is a member of `oneof`_ ``data_view``.
         spark_chart_view (google.cloud.monitoring_dashboard_v1.types.Scorecard.SparkChartView):
             Will cause the scorecard to show a spark
             chart.
 
             This field is a member of `oneof`_ ``data_view``.
-        thresholds (Sequence[google.cloud.monitoring_dashboard_v1.types.Threshold]):
-            The thresholds used to determine the state of
-            the scorecard given the time series' current
-            value. For an actual value x, the scorecard is
-            in a danger state if x is less than or equal to
-            a danger threshold that triggers below, or
-            greater than or equal to a danger threshold that
-            triggers above. Similarly, if x is above/below a
-            warning threshold that triggers above/below,
-            then the scorecard is in a warning state -
-            unless x also puts it in a danger state. (Danger
+        thresholds (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Threshold]):
+            The thresholds used to determine the state of the scorecard
+            given the time series' current value. For an actual value x,
+            the scorecard is in a danger state if x is less than or
+            equal to a danger threshold that triggers below, or greater
+            than or equal to a danger threshold that triggers above.
+            Similarly, if x is above/below a warning threshold that
+            triggers above/below, then the scorecard is in a warning
+            state - unless x also puts it in a danger state. (Danger
             trumps warning.)
-            As an example, consider a scorecard with the
-            following four thresholds: {
-              value: 90,
-              category: 'DANGER',
-              trigger: 'ABOVE',
-            },
-            {
-              value: 70,
-              category: 'WARNING',
-              trigger: 'ABOVE',
-            },
-            {
-              value: 10,
-              category: 'DANGER',
-              trigger: 'BELOW',
-            },
-            {
-              value: 20,
-              category: 'WARNING',
-              trigger: 'BELOW',
-            }
-
-            Then: values less than or equal to 10 would put
-            the scorecard in a DANGER state, values greater
-            than 10 but less than or equal to 20 a WARNING
-            state, values strictly between 20 and 70 an OK
-            state, values greater than or equal to 70 but
-            less than 90 a WARNING state, and values greater
-            than or equal to 90 a DANGER state.
+
+            As an example, consider a scorecard with the following four
+            thresholds:
+
+            ::
+
+               {
+                 value: 90,
+                 category: 'DANGER',
+                 trigger: 'ABOVE',
+               },
+               {
+                 value: 70,
+                 category: 'WARNING',
+                 trigger: 'ABOVE',
+               },
+               {
+                 value: 10,
+                 category: 'DANGER',
+                 trigger: 'BELOW',
+               },
+               {
+                 value: 20,
+                 category: 'WARNING',
+                 trigger: 'BELOW',
+               }
+
+            Then: values less than or equal to 10 would put the
+            scorecard in a DANGER state, values greater than 10 but less
+            than or equal to 20 a WARNING state, values strictly between
+            20 and 70 an OK state, values greater than or equal to 70
+            but less than 90 a WARNING state, and values greater than or
+            equal to 90 a DANGER state.
     """
 
     class GaugeView(proto.Message):
         r"""A gauge chart shows where the current value sits within a
         pre-defined range. The upper and lower bounds should define the
         possible range of values for the scorecard's query (inclusive).
 
@@ -107,19 +111,19 @@
                 or equal to this.
             upper_bound (float):
                 The upper bound for this gauge chart. The
                 value of the chart should always be less than or
                 equal to this.
         """
 
-        lower_bound = proto.Field(
+        lower_bound: float = proto.Field(
             proto.DOUBLE,
             number=1,
         )
-        upper_bound = proto.Field(
+        upper_bound: float = proto.Field(
             proto.DOUBLE,
             number=2,
         )
 
     class SparkChartView(proto.Message):
         r"""A sparkChart is a small chart suitable for inclusion in a
         table-cell or inline in text. This message contains the
@@ -136,43 +140,43 @@
                 alignment period to use in a time series query.
                 For example, if the data is published once every
                 10 minutes it would not make sense to fetch and
                 align data at one minute intervals. This field
                 is optional and exists only as a hint.
         """
 
-        spark_chart_type = proto.Field(
+        spark_chart_type: metrics.SparkChartType = proto.Field(
             proto.ENUM,
             number=1,
             enum=metrics.SparkChartType,
         )
-        min_alignment_period = proto.Field(
+        min_alignment_period: duration_pb2.Duration = proto.Field(
             proto.MESSAGE,
             number=2,
             message=duration_pb2.Duration,
         )
 
-    time_series_query = proto.Field(
+    time_series_query: metrics.TimeSeriesQuery = proto.Field(
         proto.MESSAGE,
         number=1,
         message=metrics.TimeSeriesQuery,
     )
-    gauge_view = proto.Field(
+    gauge_view: GaugeView = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="data_view",
         message=GaugeView,
     )
-    spark_chart_view = proto.Field(
+    spark_chart_view: SparkChartView = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="data_view",
         message=SparkChartView,
     )
-    thresholds = proto.RepeatedField(
+    thresholds: MutableSequence[metrics.Threshold] = proto.RepeatedField(
         proto.MESSAGE,
         number=6,
         message=metrics.Threshold,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/service.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/table.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import metrics
 from google.cloud.monitoring_dashboard_v1.types import (
     table_display_options as gmd_table_display_options,
 )
 from google.protobuf import duration_pb2  # type: ignore
@@ -30,15 +32,15 @@
 )
 
 
 class TimeSeriesTable(proto.Message):
     r"""A table that displays time series data.
 
     Attributes:
-        data_sets (Sequence[google.cloud.monitoring_dashboard_v1.types.TimeSeriesTable.TableDataSet]):
+        data_sets (MutableSequence[google.cloud.monitoring_dashboard_v1.types.TimeSeriesTable.TableDataSet]):
             Required. The data displayed in this table.
     """
 
     class TableDataSet(proto.Message):
         r"""Groups a time series query definition with table options.
 
         Attributes:
@@ -60,35 +62,37 @@
                 would not make sense to fetch and align data at one minute
                 intervals.
             table_display_options (google.cloud.monitoring_dashboard_v1.types.TableDisplayOptions):
                 Optional. Table display options for
                 configuring how the table is rendered.
         """
 
-        time_series_query = proto.Field(
+        time_series_query: metrics.TimeSeriesQuery = proto.Field(
             proto.MESSAGE,
             number=1,
             message=metrics.TimeSeriesQuery,
         )
-        table_template = proto.Field(
+        table_template: str = proto.Field(
             proto.STRING,
             number=2,
         )
-        min_alignment_period = proto.Field(
+        min_alignment_period: duration_pb2.Duration = proto.Field(
             proto.MESSAGE,
             number=3,
             message=duration_pb2.Duration,
         )
-        table_display_options = proto.Field(
-            proto.MESSAGE,
-            number=4,
-            message=gmd_table_display_options.TableDisplayOptions,
+        table_display_options: gmd_table_display_options.TableDisplayOptions = (
+            proto.Field(
+                proto.MESSAGE,
+                number=4,
+                message=gmd_table_display_options.TableDisplayOptions,
+            )
         )
 
-    data_sets = proto.RepeatedField(
+    data_sets: MutableSequence[TableDataSet] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=TableDataSet,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/table_display_options.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
-        "TableDisplayOptions",
+        "Text",
     },
 )
 
 
-class TableDisplayOptions(proto.Message):
-    r"""Table display options that can be reused.
+class Text(proto.Message):
+    r"""A widget that displays textual content.
 
     Attributes:
-        shown_columns (Sequence[str]):
-            Optional. This field is unused and has been replaced by
-            TimeSeriesTable.column_settings
+        content (str):
+            The text content to be displayed.
+        format (~.text.Text.Format):
+            How the text content is formatted.
     """
 
-    shown_columns = proto.RepeatedField(
-        proto.STRING,
-        number=1,
+    class Format(proto.Enum):
+        r"""The format type of the text content."""
+        FORMAT_UNSPECIFIED = 0
+        MARKDOWN = 1
+        RAW = 2
+
+    content = proto.Field(proto.STRING, number=1)
+
+    format = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=Format,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/text.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/text.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
         "Text",
@@ -36,19 +38,19 @@
 
     class Format(proto.Enum):
         r"""The format type of the text content."""
         FORMAT_UNSPECIFIED = 0
         MARKDOWN = 1
         RAW = 2
 
-    content = proto.Field(
+    content: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    format_ = proto.Field(
+    format_: Format = proto.Field(
         proto.ENUM,
         number=2,
         enum=Format,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/widget.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import alertchart
 from google.cloud.monitoring_dashboard_v1.types import (
     collapsible_group as gmd_collapsible_group,
 )
 from google.cloud.monitoring_dashboard_v1.types import logs_panel as gmd_logs_panel
@@ -83,61 +85,61 @@
             This field is a member of `oneof`_ ``content``.
         logs_panel (google.cloud.monitoring_dashboard_v1.types.LogsPanel):
             A widget that shows a stream of logs.
 
             This field is a member of `oneof`_ ``content``.
     """
 
-    title = proto.Field(
+    title: str = proto.Field(
         proto.STRING,
         number=1,
     )
-    xy_chart = proto.Field(
+    xy_chart: xychart.XyChart = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="content",
         message=xychart.XyChart,
     )
-    scorecard = proto.Field(
+    scorecard: gmd_scorecard.Scorecard = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="content",
         message=gmd_scorecard.Scorecard,
     )
-    text = proto.Field(
+    text: gmd_text.Text = proto.Field(
         proto.MESSAGE,
         number=4,
         oneof="content",
         message=gmd_text.Text,
     )
-    blank = proto.Field(
+    blank: empty_pb2.Empty = proto.Field(
         proto.MESSAGE,
         number=5,
         oneof="content",
         message=empty_pb2.Empty,
     )
-    alert_chart = proto.Field(
+    alert_chart: alertchart.AlertChart = proto.Field(
         proto.MESSAGE,
         number=7,
         oneof="content",
         message=alertchart.AlertChart,
     )
-    time_series_table = proto.Field(
+    time_series_table: table.TimeSeriesTable = proto.Field(
         proto.MESSAGE,
         number=8,
         oneof="content",
         message=table.TimeSeriesTable,
     )
-    collapsible_group = proto.Field(
+    collapsible_group: gmd_collapsible_group.CollapsibleGroup = proto.Field(
         proto.MESSAGE,
         number=9,
         oneof="content",
         message=gmd_collapsible_group.CollapsibleGroup,
     )
-    logs_panel = proto.Field(
+    logs_panel: gmd_logs_panel.LogsPanel = proto.Field(
         proto.MESSAGE,
         number=10,
         oneof="content",
         message=gmd_logs_panel.LogsPanel,
     )
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/cloud/monitoring_dashboard_v1/types/xychart.py` & `google-cloud-monitoring-dashboards-2.9.0/google/cloud/monitoring_dashboard_v1/types/xychart.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from typing import MutableMapping, MutableSequence
+
 import proto  # type: ignore
 
 from google.cloud.monitoring_dashboard_v1.types import metrics
 from google.protobuf import duration_pb2  # type: ignore
 
 
 __protobuf__ = proto.module(
@@ -28,25 +30,25 @@
 )
 
 
 class XyChart(proto.Message):
     r"""A chart that displays data on a 2D (X and Y axes) plane.
 
     Attributes:
-        data_sets (Sequence[google.cloud.monitoring_dashboard_v1.types.XyChart.DataSet]):
+        data_sets (MutableSequence[google.cloud.monitoring_dashboard_v1.types.XyChart.DataSet]):
             Required. The data displayed in this chart.
         timeshift_duration (google.protobuf.duration_pb2.Duration):
             The duration used to display a comparison
             chart. A comparison chart simultaneously shows
             values from two similar-length time periods
             (e.g., week-over-week metrics).
             The duration must be positive, and it can only
             be applied to charts with data sets of LINE plot
             type.
-        thresholds (Sequence[google.cloud.monitoring_dashboard_v1.types.Threshold]):
+        thresholds (MutableSequence[google.cloud.monitoring_dashboard_v1.types.Threshold]):
             Threshold lines drawn horizontally across the
             chart.
         x_axis (google.cloud.monitoring_dashboard_v1.types.XyChart.Axis):
             The properties applied to the X axis.
         y_axis (google.cloud.monitoring_dashboard_v1.types.XyChart.Axis):
             The properties applied to the Y axis.
         y2_axis (google.cloud.monitoring_dashboard_v1.types.XyChart.Axis):
@@ -92,34 +94,34 @@
 
         class TargetAxis(proto.Enum):
             r"""An axis identifier."""
             TARGET_AXIS_UNSPECIFIED = 0
             Y1 = 1
             Y2 = 2
 
-        time_series_query = proto.Field(
+        time_series_query: metrics.TimeSeriesQuery = proto.Field(
             proto.MESSAGE,
             number=1,
             message=metrics.TimeSeriesQuery,
         )
-        plot_type = proto.Field(
+        plot_type: "XyChart.DataSet.PlotType" = proto.Field(
             proto.ENUM,
             number=2,
             enum="XyChart.DataSet.PlotType",
         )
-        legend_template = proto.Field(
+        legend_template: str = proto.Field(
             proto.STRING,
             number=3,
         )
-        min_alignment_period = proto.Field(
+        min_alignment_period: duration_pb2.Duration = proto.Field(
             proto.MESSAGE,
             number=4,
             message=duration_pb2.Duration,
         )
-        target_axis = proto.Field(
+        target_axis: "XyChart.DataSet.TargetAxis" = proto.Field(
             proto.ENUM,
             number=5,
             enum="XyChart.DataSet.TargetAxis",
         )
 
     class Axis(proto.Message):
         r"""A chart axis.
@@ -134,55 +136,55 @@
 
         class Scale(proto.Enum):
             r"""Types of scales used in axes."""
             SCALE_UNSPECIFIED = 0
             LINEAR = 1
             LOG10 = 2
 
-        label = proto.Field(
+        label: str = proto.Field(
             proto.STRING,
             number=1,
         )
-        scale = proto.Field(
+        scale: "XyChart.Axis.Scale" = proto.Field(
             proto.ENUM,
             number=2,
             enum="XyChart.Axis.Scale",
         )
 
-    data_sets = proto.RepeatedField(
+    data_sets: MutableSequence[DataSet] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message=DataSet,
     )
-    timeshift_duration = proto.Field(
+    timeshift_duration: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=4,
         message=duration_pb2.Duration,
     )
-    thresholds = proto.RepeatedField(
+    thresholds: MutableSequence[metrics.Threshold] = proto.RepeatedField(
         proto.MESSAGE,
         number=5,
         message=metrics.Threshold,
     )
-    x_axis = proto.Field(
+    x_axis: Axis = proto.Field(
         proto.MESSAGE,
         number=6,
         message=Axis,
     )
-    y_axis = proto.Field(
+    y_axis: Axis = proto.Field(
         proto.MESSAGE,
         number=7,
         message=Axis,
     )
-    y2_axis = proto.Field(
+    y2_axis: Axis = proto.Field(
         proto.MESSAGE,
         number=9,
         message=Axis,
     )
-    chart_options = proto.Field(
+    chart_options: "ChartOptions" = proto.Field(
         proto.MESSAGE,
         number=8,
         message="ChartOptions",
     )
 
 
 class ChartOptions(proto.Message):
@@ -196,15 +198,15 @@
     class Mode(proto.Enum):
         r"""Chart mode options."""
         MODE_UNSPECIFIED = 0
         COLOR = 1
         X_RAY = 2
         STATS = 3
 
-    mode = proto.Field(
+    mode: Mode = proto.Field(
         proto.ENUM,
         number=1,
         enum=Mode,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/async_client.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/client.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/pagers.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/base.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/services/dashboards_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/common.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/dashboard.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/dashboard.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/dashboards_service.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/dashboards_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/drilldowns.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/drilldowns.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/layouts.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/layouts.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/metrics.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/metrics.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/scorecard.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/scorecard.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/service.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/text.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,41 +14,71 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import proto  # type: ignore
 
 
+from google.monitoring.dashboard_v1.types import scorecard as gmd_scorecard
+from google.monitoring.dashboard_v1.types import text as gmd_text
+from google.monitoring.dashboard_v1.types import xychart
+from google.protobuf import empty_pb2 as empty  # type: ignore
+
+
 __protobuf__ = proto.module(
     package="google.monitoring.dashboard.v1",
     manifest={
-        "Text",
+        "Widget",
     },
 )
 
 
-class Text(proto.Message):
-    r"""A widget that displays textual content.
+class Widget(proto.Message):
+    r"""Widget contains a single dashboard component and
+    configuration of how to present the component in the dashboard.
 
     Attributes:
-        content (str):
-            The text content to be displayed.
-        format (~.text.Text.Format):
-            How the text content is formatted.
+        title (str):
+            Optional. The title of the widget.
+        xy_chart (~.xychart.XyChart):
+            A chart of time series data.
+        scorecard (~.gmd_scorecard.Scorecard):
+            A scorecard summarizing time series data.
+        text (~.gmd_text.Text):
+            A raw string or markdown displaying textual
+            content.
+        blank (~.empty.Empty):
+            A blank space.
     """
 
-    class Format(proto.Enum):
-        r"""The format type of the text content."""
-        FORMAT_UNSPECIFIED = 0
-        MARKDOWN = 1
-        RAW = 2
-
-    content = proto.Field(proto.STRING, number=1)
+    title = proto.Field(proto.STRING, number=1)
 
-    format = proto.Field(
-        proto.ENUM,
+    xy_chart = proto.Field(
+        proto.MESSAGE,
         number=2,
-        enum=Format,
+        oneof="content",
+        message=xychart.XyChart,
+    )
+
+    scorecard = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        oneof="content",
+        message=gmd_scorecard.Scorecard,
+    )
+
+    text = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        oneof="content",
+        message=gmd_text.Text,
+    )
+
+    blank = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        oneof="content",
+        message=empty.Empty,
     )
 
 
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google/monitoring/dashboard_v1/types/xychart.py` & `google-cloud-monitoring-dashboards-2.9.0/google/monitoring/dashboard_v1/types/xychart.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/PKG-INFO` & `google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: google-cloud-monitoring-dashboards
-Version: 2.8.0
-Summary: Monitoring Dashboards API client library
+Version: 2.9.0
+Summary: Google Cloud Monitoring Dashboards API client library
 Home-page: https://github.com/googleapis/python-monitoring-dashboards
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/google_cloud_monitoring_dashboards.egg-info/SOURCES.txt` & `google-cloud-monitoring-dashboards-2.9.0/google_cloud_monitoring_dashboards.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 google/cloud/monitoring_dashboard/__init__.py
+google/cloud/monitoring_dashboard/gapic_version.py
 google/cloud/monitoring_dashboard/py.typed
 google/cloud/monitoring_dashboard/v1/proto/common.proto
 google/cloud/monitoring_dashboard/v1/proto/dashboard.proto
 google/cloud/monitoring_dashboard/v1/proto/dashboards_service.proto
 google/cloud/monitoring_dashboard/v1/proto/drilldowns.proto
 google/cloud/monitoring_dashboard/v1/proto/layouts.proto
 google/cloud/monitoring_dashboard/v1/proto/metrics.proto
 google/cloud/monitoring_dashboard/v1/proto/scorecard.proto
 google/cloud/monitoring_dashboard/v1/proto/service.proto
 google/cloud/monitoring_dashboard/v1/proto/text.proto
 google/cloud/monitoring_dashboard/v1/proto/widget.proto
 google/cloud/monitoring_dashboard/v1/proto/xychart.proto
 google/cloud/monitoring_dashboard_v1/__init__.py
 google/cloud/monitoring_dashboard_v1/gapic_metadata.json
+google/cloud/monitoring_dashboard_v1/gapic_version.py
 google/cloud/monitoring_dashboard_v1/py.typed
 google/cloud/monitoring_dashboard_v1/services/__init__.py
 google/cloud/monitoring_dashboard_v1/services/dashboards_service/__init__.py
 google/cloud/monitoring_dashboard_v1/services/dashboards_service/async_client.py
 google/cloud/monitoring_dashboard_v1/services/dashboards_service/client.py
 google/cloud/monitoring_dashboard_v1/services/dashboards_service/pagers.py
 google/cloud/monitoring_dashboard_v1/services/dashboards_service/transports/__init__.py
@@ -74,13 +76,14 @@
 google_cloud_monitoring_dashboards.egg-info/PKG-INFO
 google_cloud_monitoring_dashboards.egg-info/SOURCES.txt
 google_cloud_monitoring_dashboards.egg-info/dependency_links.txt
 google_cloud_monitoring_dashboards.egg-info/namespace_packages.txt
 google_cloud_monitoring_dashboards.egg-info/not-zip-safe
 google_cloud_monitoring_dashboards.egg-info/requires.txt
 google_cloud_monitoring_dashboards.egg-info/top_level.txt
-scripts/fixup_dashboard_v1_keywords.py
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/dashboard_v1/__init__.py
-tests/unit/gapic/dashboard_v1/test_dashboards_service.py
+tests/unit/gapic/dashboard_v1/test_dashboards_service.py
+tests/unit/gapic/monitoring_dashboard_v1/__init__.py
+tests/unit/gapic/monitoring_dashboard_v1/test_dashboards_service.py
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/setup.py` & `google-cloud-monitoring-dashboards-2.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 # -*- coding: utf-8 -*-
-#
-# Copyright 2020 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import io
 import os
 
-import setuptools
+import setuptools  # type: ignore
 
+package_root = os.path.abspath(os.path.dirname(__file__))
 
 name = "google-cloud-monitoring-dashboards"
-description = "Monitoring Dashboards API client library"
-version = "2.8.0"
-release_status = "Development Status :: 5 - Production/Stable"
+
+
+description = "Google Cloud Monitoring Dashboards API client library"
+
+version = {}
+with open(
+    os.path.join(package_root, "google/cloud/monitoring_dashboard/gapic_version.py")
+) as fp:
+    exec(fp.read(), version)
+version = version["__version__"]
+
+if version[0] == "0":
+    release_status = "Development Status :: 4 - Beta"
+else:
+    release_status = "Development Status :: 5 - Production/Stable"
+
 dependencies = [
-    "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
+    "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
+url = "https://github.com/googleapis/python-monitoring-dashboards"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -50,15 +64,15 @@
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="googleapis-packages@google.com",
     license="Apache 2.0",
-    url="https://github.com/googleapis/python-monitoring-dashboards",
+    url=url,
     classifiers=[
         release_status,
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -66,14 +80,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
         "Topic :: Internet",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
+    python_requires=">=3.7",
     namespace_packages=namespaces,
     install_requires=dependencies,
-    python_requires=">=3.7",
-    scripts=["scripts/fixup_dashboard_v1_keywords.py"],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `google-cloud-monitoring-dashboards-2.8.0/tests/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/tests/unit/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/dashboard_v1/__init__.py` & `google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/dashboard_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-monitoring-dashboards-2.8.0/tests/unit/gapic/dashboard_v1/test_dashboards_service.py` & `google-cloud-monitoring-dashboards-2.9.0/tests/unit/gapic/dashboard_v1/test_dashboards_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 from google.cloud.monitoring_dashboard_v1.types import table
 from google.cloud.monitoring_dashboard_v1.types import table_display_options
 from google.cloud.monitoring_dashboard_v1.types import text
 from google.cloud.monitoring_dashboard_v1.types import widget
 from google.cloud.monitoring_dashboard_v1.types import xychart
 from google.oauth2 import service_account
 from google.protobuf import duration_pb2  # type: ignore
+from google.protobuf import empty_pb2  # type: ignore
 import google.auth
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
```

